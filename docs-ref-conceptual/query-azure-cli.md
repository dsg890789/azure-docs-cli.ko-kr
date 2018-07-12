---
title: Azure CLI 2.0을 사용한 쿼리 명령 결과
description: Azure CLI 2.0 명령의 출력에 대해 JMESPath 쿼리를 수행하는 방법을 학습합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 97fcd9d5b5a65480957734cec0ead68029918a49
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967795"
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Azure CLI 2.0과 함께 JMESPath 쿼리 사용

Azure CLI 2.0은 `--query` 인수를 사용하여 명령의 결과에 대해 [JMESPath 쿼리](http://jmespath.org)를 실행합니다. JMESPath는 JSON의 쿼리 언어이며, CLI 출력의 데이터를 선택하고 표시하는 기능을 제공합니다. 다른 표시 형식을 지정하기 전에 이러한 쿼리를 JSON 출력에서 실행합니다.

`--query` 인수는 Azure CLI의 모든 명령에서 지원됩니다. 이 문서의 예제는 일반적인 사용 사례를 다루고 JMESPath 기능을 사용하는 방법을 보여줍니다.

## <a name="work-with-dictionary-output"></a>사전 출력으로 작업

JSON 사전을 반환하는 명령을 해당 키 이름만으로 탐색할 수 있습니다. 키 경로는 `.` 문자를 구분 기호로 사용합니다. 다음 예제에서는 Linux VM에 연결할 수 있도록 허용된 공용 SSH 키 목록을 끌어옵니다.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

또한 여러 값을 가져와서 정렬된 배열에 배치할 수 있습니다. 배열에는 키 정보가 없지만 배열의 요소 순서는 쿼리된 키 순서와 일치하지 않습니다. 다음 예제에서는 OS 디스크의 이름 및 크기를 제공하는 Azure 이미지를 검색하는 방법을 보여줍니다.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

출력에 키를 배치하는 경우 대체 사전 구문을 사용할 수 있습니다. 사전에 대한 여러 요소 선택 영역은 `{displayKey:keyPath, ...}` 형식을 사용하여 `keyPath` JMESPath 식으로 필터링합니다. 그러면 출력에 `{displayKey: value}`로 표시됩니다. 다음 예제에서는 마지막 예제의 쿼리를 사용하고 출력에 키를 할당하여 더 명확하게 합니다.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

`table` 출력 형식으로 정보를 표시할 때 사전 표시가 특히 유용합니다. 이렇게 하면 고유한 열 헤드가 출력을 쉽게 읽을 수 있도록 설정합니다. 출력 형식에 대한 자세한 내용은 [Azure CLI 2.0 명령에 대한 출력 형식](/cli/azure/format-output-azure-cli)을 참조하세요.

> [!NOTE]
> 특정 키는 필터링되고 테이블 보기에 인쇄되지 않습니다. 이러한 키는 `id`, `type` 및 `etag`입니다. 이 정보를 표시해야 하는 경우 키 이름을 변경하고 필터링하지 않을 수 있습니다.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>목록 출력으로 작업

하나 이상의 값을 반환할 수 있는 CLI 명령은 항상 배열을 반환합니다. 배열은 인덱스가 해당 요소에 액세스하도록 할 수 있지만 CLI에서 순서를 보장하지 않습니다. 값의 배열을 쿼리하는 가장 좋은 방법은 `[]` 연산자를 사용하여 평면화하는 것입니다. 연산자는 배열의 키 이후에 또는 식의 첫 번째 요소로 작성됩니다. 평면화는 배열에서 각 개별 요소에서 쿼리를 실행하고 결과 값을 새 배열에 배치합니다. 다음 예제에서는 리소스 그룹의 각 VM에서 실행 중인 이름 및 OS를 인쇄합니다.

```azurecli-interactive
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

키 경로의 일부인 배열도 평면화될 수 있습니다. 이 예제에서는 VM이 연결된 NIC의 Azure 개체 ID를 가져오는 쿼리를 보여줍니다.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>조건자를 사용하여 배열 출력 필터링

JMESPath는 [필터링 식](http://jmespath.org/specification.html#filterexpressions)을 제공하여 표시된 데이터를 필터링합니다. 이러한 식은 [JMESPath 기본 제공 함수](http://jmespath.org/specification.html#built-in-functions)와 함께 결합되어 부분적으로 일치를 수행하거나 표준 형식으로 데이터를 조작할 경우에 특히 강력합니다. 필터 식은 배열 데이터에서만 작동하고 다른 상황에서 사용될 때 `null` 값을 반환합니다. 예를 들어 `vm list`와 같은 명령의 출력을 사용하고 필터링하여 특정 형식의 VM을 찾을 수 있습니다. 다음 예제에서는 Windows VM만을 캡처하고 해당 이름을 인쇄하도록 VM 형식을 필터링하여 이전 항목으로 확장합니다.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>대화형으로 쿼리를 사용하여 실험

JMESPath 식을 사용하여 실험하려면 신속하게 쿼리를 편집하고 출력을 검사할 수 있는 방식으로 작업합니다. 
  [JMESPath 터미널](https://github.com/jmespath/jmespath.terminal) Python 패키지에서 대화형 환경을 제공합니다. 이 기능은 데이터를 추출하기 위해 데이터를 입력으로 파이핑한 다음, 프로그램 내 쿼리를 작성하는 데 사용됩니다.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

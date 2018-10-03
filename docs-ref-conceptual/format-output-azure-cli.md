---
title: Azure CLI의 출력 형식
description: Azure CLI 명령 출력을 테이블, 목록 또는 json 형식으로 지정하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5b5d962e244037d9c904fc5c75314661130d1910
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178068"
---
# <a name="output-formats-for-azure-cli-commands"></a>Azure CLI 명령의 출력 형식

Azure CLI는 기본 출력 형식으로 JSON을 사용하지만 다른 형식도 제공합니다.  `--output`(`--out` 또는 `-o`) 매개 변수를 사용하여 CLI 출력의 형식을 지정합니다. 인수 값과 출력의 형식은 다음과 같습니다.

--output | 설명
---------|-------------------------------
`json`   | JSON 문자열 이 설정은 기본값입니다.
`jsonc`  | 색으로 구분된 JSON
`yaml`   | 머신이 읽을 수 있는 JSON 대안인 YAML.
`table`  | 열 제목인 키가 포함된 ASCII 테이블
`tsv`    | 키가 포함되지 않은 탭으로 구분된 값

## <a name="json-output-format"></a>JSON 출력 형식

다음 예제에서는 구독의 가상 머신 목록을 기본 json 형식으로 표시합니다.

```azurecli-interactive
az vm list --output json
```

다음과 같은 출력에는 편의를 위해 생략되고, 교체된 정보를 식별하는 몇몇 필드가 있습니다.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="yaml-output-format"></a>YAML 출력 형식

`yaml` 형식은 출력을 일반 텍스트 데이터 serialization 형식인 [YAML](http://yaml.org/)로 인쇄합니다. YAML은 JSON보다 읽기 쉬우며, 해당 형식으로 쉽게 매핑됩니다. 일부 응용 프로그램 및 CLI 명령은 JSON 대신 YAML을 구성 입력으로 사용합니다.

```azurecli-interactive
az vm list --out yaml
```

다음과 같은 출력에는 편의를 위해 생략되고, 교체된 정보를 식별하는 몇몇 필드가 있습니다.

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a>테이블 출력 형식

`table` 형식은 ASCII 테이블로 출력을 인쇄하여 읽고 검사하기 쉽게 합니다. 중첩된 개체는 테이블 출력에 포함되지 않지만 쿼리의 일부로 필터링될 수 있습니다. 일부 필드는 테이블에 포함되지 않습니다. 따라서 빠르고 검색 가능한 데이터의 개요를 만들려는 경우 이 형식을 사용하는 것이 좋습니다.

```azurecli-interactive
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

`--query` 매개 변수를 사용하여 목록 출력에 표시할 속성과 열을 사용자 지정할 수 있습니다. 다음 예제에서는 `list` 명령에서 VM 이름 및 리소스 그룹 이름만 선택하는 방법을 보여 줍니다.

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> 일부 키는 기본적으로 테이블 보기에 인쇄되지 않습니다. `id`, `type` 및 `etag`가 포함됩니다. 출력에 표시해야 하는 경우 JMESPath 리키잉 기능을 사용하여 키 이름을 변경하고 필터링을 방지할 수 있습니다.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

데이터를 필터링하는 쿼리를 사용하는 방법에 대한 자세한 내용은 [Azure CLI와 함께 JMESPath 쿼리 사용](/cli/azure/query-azure-cli)을 참조하세요.

## <a name="tsv-output-format"></a>TSV 출력 형식

`tsv` 출력 형식은 추가 서식 지정, 키 또는 다른 기호 없이 탭 및 줄 바꿈으로 구분된 값을 반환합니다. 이 형식은 출력을 어떤 형태의 텍스트를 처리해야 하는 다른 명령 및 도구에 간편하게 사용할 수 있습니다. `table` 형식과 마찬가지로 `tsv`는 중첩된 개체를 인쇄하지 않습니다.

앞의 예제에 `tsv` 옵션을 사용하면 탭으로 구분된 결과가 출력됩니다.

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

다음 예제는 `tsv` 출력이 bash에서 다른 명령에 파이프되는 방법을 보여줍니다. `grep`은 이름에 "RGD"라는 텍스트가 포함된 항목을 선택하고, `cut` 명령은 8번째 필드를 선택하여 출력에 VM 이름을 표시합니다.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

값은 탭으로 구분된 필드를 처리할 용도로 인쇄된 JSON 개체에 표시되는 것과 동일한 순서입니다. 이 순서는 명령에서 일관되게 실행되도록 보장됩니다.

## <a name="set-the-default-output-format"></a>기본 출력 형식을 설정합니다.

대화형 `az configure` 명령을 사용하여 환경을 설정하고 출력 형식에 대한 기본 설정을 지정합니다. 기본 출력 형식은 `json`입니다.

```azurecli-interactive
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

환경을 구성하는 방법에 대해 자세히 알아보려면 [Azure CLI 구성](/cli/azure/azure-cli-configuration)을 참조하세요.

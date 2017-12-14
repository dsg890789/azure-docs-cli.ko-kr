---
title: "Azure CLI 2.0 대화형 모드"
description: "대화형 모드에서 Azure CLI 2.0을 사용합니다."
keywords: "Azure CLI 2.0, 대화형 모드"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 
ms.openlocfilehash: fb260d7385728acd0c699488ecb5b108afefd08c
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="interactive-azure-cli-20"></a>대화형 Azure CLI 2.0

`az interactive` 명령을 실행하여 대화형 모드에서 Azure CLI 2.0을 사용할 수 있습니다.
그러면 명령이 자동으로 완성되고, 명령 및 해당 매개 변수에 대한 설명과 명령 예제에 액세스할 수 있는 대화형 셸로 이동됩니다.

![대화형 모드](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> 여기서는 검은색 배경에서는 잘 보이지 않는 기본 스타일을 사용하지 않습니다.

계정에 아직 로그인하지 않은 경우 `login` 명령을 사용하여 로그인합니다.

## <a name="configure"></a>구성

대화형 모드는 필요에 따라 명령 설명, 매개 변수 설명 및 명령 예제를 표시합니다.
`F1` 키를 사용해서 설명 및 예제를 표시하거나 표시하지 않을 수 있습니다.

![설명 및 예제](./media/interactive-azure-cli/descriptions-and-examples.png)

`F2` 키를 사용하여 매개 변수 기본값을 표시하거나 표시하지 않을 수 있습니다.

![기본값](./media/interactive-azure-cli/defaults.png)

`F3` 키는 일부 키 제스처를 표시하거나 숨깁니다.

![제스처](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a>범위

대화형 모드의 범위를 `vm` 또는 `vm image`와 같은 특정 명령 그룹으로 지정할 수 있습니다.
이렇게 하면 해당 범위에서 모든 명령이 해석됩니다.
해당 명령 그룹에서 모든 작업을 수행하려는 경우에는 이 방법이 간단합니다.

다음 명령을 입력하는 대신

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

vm 명령 그룹으로 범위를 지정하고 다음 명령을 입력할 수 잇습니다.

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

하위 수준 명령 그룹으로도 범위를 지정할 수 있습니다.
`%%vm image`를 사용하여 `vm image`로 범위를 지정할 수 있습니다.
이 경우 이미 `vm`으로 범위를 지정했으므로 `%%image`를 사용할 수 있습니다.

```azurecli
az vm>> %%image
az vm image>>
```

이때 `%%..`를 사용하여 범위를 `vm`으로 다시 되돌리거나 `%%`만 사용해서 범위를 루트로 지정할 수 있습니다.

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a>쿼리

실행한 마지막 명령의 결과에 대해 JMESPath 쿼리를 실행할 수 있습니다.
예를 들어 VM을 만든 후 완전히 프로비전되었는지 확인할 수 있습니다.

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

명령의 결과를 쿼리하는 방법에 대한 자세한 내용은 [Azure 2.0을 사용한 쿼리 명령 결과](query-azure-cli.md)를 참조하세요.

## <a name="bash-commands"></a>Bash 명령

`#[cmd]` 명령을 사용하여 대화형 모드를 종료하지 않고 셸 명령을 실행할 수 있습니다.

```azurecli
az>> #dir
```

## <a name="examples"></a>예

일부 명령에는 많은 예제가 있습니다.
`CTRL-N`을 사용하여 예제의 다음 페이지로 스크롤하거나, `CTRL-Y`를 사용하여 예제의 이전 페이지로 스크롤할 수 있습니다.

![예제](./media/interactive-azure-cli/examples.png)

`::#`을 사용하여 구체적인 예제를 살펴볼 수도 있습니다.

```azurecli
az>> vm create ::8
```

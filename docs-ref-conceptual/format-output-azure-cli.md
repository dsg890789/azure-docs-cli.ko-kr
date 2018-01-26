---
title: "Azure CLI 2.0의 출력 형식"
description: "--output을 사용하여 Azure CLI 2.0 명령의 출력을 테이블, 목록 또는 json 형식으로 지정합니다."
keywords: "Azure CLI 2.0, 출력, 형식, 테이블, 목록, json, Linux, Mac, Windows, OS X"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 74bdb727-481d-45f7-a44e-15d18dc55483
ms.openlocfilehash: 3e99c2533031dc063a50996f26712d4df92f65c9
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Azure CLI 2.0 명령의 출력 형식

Azure CLI 2.0은 기본 출력 옵션으로 json을 사용하지만 모든 명령의 출력 형식을 지정하는 다양한 방법을 제공합니다.  `--output`(또는 `--out` 또는 `-o`) 매개 변수를 사용하여 명령의 출력을 다음 테이블에 나와 있는 출력 형식 중 하나로 지정합니다.

--output | 설명
---------|-------------------------------
`json`   | json 문자열입니다. 기본값은 `json`입니다.
`jsonc`  | 색으로 구분된 json 문자열입니다.
`table`  | 열 머리글이 있는 테이블입니다.
`tsv`    | 탭으로 구분된 값입니다.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a>Json 옵션 사용

다음 예제에서는 구독의 가상 컴퓨터 목록을 기본 json 형식으로 표시합니다.

```azurecli-interactive
az vm list --output json
```

결과는 이 형식(간단하게 표시하기 위해 출력의 일부만 표시)입니다.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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

## <a name="using-the-table-option"></a>테이블 옵션 사용

테이블 옵션은 읽기 쉬운 출력 집합을 제공하지만, 이전의 json 예제와는 달리 중첩된 개체는 단순 `--output table`을 사용하는 출력에 포함되지 않습니다.  '테이블' 출력 형식의 동일한 예제를 사용하면 가장 일반적인 속성 값 큐 레이트 목록이 제공됩니다.

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

`--query` 매개 변수를 사용하여 목록 출력에 표시할 속성과 열을 사용자 지정할 수 있습니다. 다음 예제에서는 `list` 명령에서 VM 이름 및 리소스 그룹 이름만 선택하는 방법을 보여 줍니다.

```azurecli-interactive
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a>tsv 옵션 사용

'tsv' 출력 형식은 머리글과 대시 없이 간단한 텍스트 기반의 탭으로 구분된 출력을 반환합니다. 이 형식은 출력을 어떤 형태의 텍스트를 처리해야 하는 다른 명령 및 도구에 간편하게 사용할 수 있습니다. 앞의 예제에 `tsv` 옵션을 사용하면 탭으로 구분된 결과가 출력됩니다.

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

다음 예제에서는 `tsv` 출력을 `grep` 및 `cut` 같은 명령으로 전달하여 `list` 출력의 특정 값을 자세히 구문 분석하는 방법을 보여 줍니다. `grep` 명령은 이름에 "RGD"라는 텍스트가 포함된 항목만 선택하고, `cut` 명령은 8번째 필드(탭으로 구분됨) 값만 선택하여 출력에 표시합니다.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>기본 출력 형식 설정

`az configure` 명령을 사용하여 환경을 설정하거나 출력 형식에 대한 기본 설정과 같은 기본 설정을 구성할 수 있습니다. 일반적인 예로, 가장 간단한 출력 형식 기본값은 "테이블" 형식입니다. 출력 형식을 선택하라는 메시지가 표시되면 **3**을 선택하면 됩니다.

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]:
```
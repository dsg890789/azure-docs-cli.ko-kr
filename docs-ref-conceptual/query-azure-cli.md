---
title: "Azure CLI 2.0을 사용한 쿼리 명령 결과"
description: "Azure CLI 2.0 명령의 출력에 대해 JMESPath 쿼리를 수행하는 방법을 학습합니다."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98bc35c1e8136231011a2303901f42c68c9a7758
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Azure CLI 2.0과 함께 JMESPath 쿼리 사용

Azure CLI 2.0은 `--query` 매개 변수를 사용하여 `az` 명령의 결과에 대해 [JMESPath 쿼리](http://jmespath.org)를 수행합니다. JMESPath는 JSON 출력에 대한 강력한 쿼리 언어입니다.  JMESPath 쿼리에 대해 잘 모르는 경우 [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html)에서 자습서를 찾을 수 있습니다.

`Query` 매개 변수는 Azure CLI 2.0 내의 모든 리소스 유형(컨테이너 서비스, Web Apps, VM 등)에서 지원되며 다양한 용도로 사용할 수 있습니다.  아래에 몇 가지 예가 나열되어 있습니다.

## <a name="select-simple-properties"></a>단순 속성 선택

출력 형식이 `table`인 단순 `list` 명령은 각 리소스 유형에 대한 가장 일반적이고 간단한 큐 레이트 속성 집합을 읽기 쉬운 테이블 형식으로 반환합니다.

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

`--query` 매개 변수를 사용하여 구독의 모든 가상 컴퓨터에 대 한 리소스 그룹 이름과 VM 이름만을 표시할 수 있습니다.

```azurecli-interactive
az vm list \
  --query "[].[name, resourceGroup]" --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

이전 예제에서는 열 머리글이 "Column1" 및 "Column2" 였습니다.  사용자는 선택한 속성에 익숙한 레이블 또는 이름을 추가할 수 있습니다.  다음 예제에서는 선택한 속성 "name" 및 "resourceGroup"에 "VMName" 및 "RGName" 레이블을 추가했습니다.


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="select-complex-nested-properties"></a>복잡한 중첩 속성 선택

선택하려는 속성이 JSON 출력에서 깊숙이 중첩된 경우 해당 중첩 속성의 전체 경로를 제공해야 합니다. 다음 예제에서는 vm 목록 명령에서 VMName 및 OS 유형을 선택하는 방법을 보여 줍니다.

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a>contains 함수로 필터링

JMESPath `contains` 함수를 사용하여 쿼리에서 반환된 결과를 구체화할 수 있습니다.
다음 예제의 명령은 이름에 "RGD"라는 텍스트가 포함된 VM만 선택합니다.

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

다음 예제의 결과는 vmSize 'Standard_DS1'이 포함된 VM을 반환합니다.

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a>grep를 사용하여 필터링

`tsv` 출력 형식은 헤더 없이 탭으로 구분된 텍스트입니다. `grep` 및 `cut` 같은 명령으로 전달하여 `list` 출력의 특정 값을 자세히 구문 분석할 수 있습니다. 다음 예제의 `grep` 명령은 이름에 "RGD"라는 텍스트가 포함된 VM만 선택합니다.  `cut` 명령은 8번째 필드(탭으로 구분됨) 값만 선택하여 출력에 표시합니다.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Jpterm을 사용하여 탐색

명령 출력을 [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal)로 전달하고 거기서 JMESPath 쿼리를 실험할 수도 있습니다.

```bash
pip install jmespath-terminal
az vm list | jpterm
```


---
title: "Azure CLI 2.0을 사용한 쿼리 명령 결과"
description: "Azure CLI 2.0 명령의 출력에 대해 JMESPath 쿼리를 수행하려면 --query를 사용합니다."
keywords: "Azure CLI 2.0, JMESPath, 쿼리, Linux, Mac, Windows, OS X"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: 8ab4a5e38f06199c5f044b8526c581828ba61927
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/18/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="b38ce-104">Azure CLI 2.0과 함께 JMESPath 쿼리 사용</span><span class="sxs-lookup"><span data-stu-id="b38ce-104">Using JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="b38ce-105">Azure CLI 2.0은 `--query` 매개 변수를 사용하여 `az` 명령의 결과에 대해 [JMESPath 쿼리](http://jmespath.org)를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-105">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="b38ce-106">JMESPath는 JSON 출력에 대한 강력한 쿼리 언어입니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-106">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="b38ce-107">JMESPath 쿼리에 대해 잘 모르는 경우 [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html)에서 자습서를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-107">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="b38ce-108">`Query` 매개 변수는 Azure CLI 2.0 내의 모든 리소스 유형(컨테이너 서비스, Web Apps, VM 등)에서 지원되며 다양한 용도로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-108">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="b38ce-109">아래에 몇 가지 예가 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-109">We have listed several examples below.</span></span>

## <a name="selecting-simple-properties"></a><span data-ttu-id="b38ce-110">단순 속성 선택</span><span class="sxs-lookup"><span data-stu-id="b38ce-110">Selecting simple properties</span></span>

<span data-ttu-id="b38ce-111">출력 형식이 `table`인 단순 `list` 명령은 각 리소스 유형에 대한 가장 일반적이고 간단한 큐 레이트 속성 집합을 읽기 쉬운 테이블 형식으로 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-111">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

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

<span data-ttu-id="b38ce-112">`--query` 매개 변수를 사용하여 구독의 모든 가상 컴퓨터에 대 한 리소스 그룹 이름과 VM 이름만을 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-112">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query [*].[name, resourceGroup] --out table
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

<span data-ttu-id="b38ce-113">이전 예제에서는 열 머리글이 "Column1" 및 "Column2" 였습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-113">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="b38ce-114">사용자는 선택한 속성에 익숙한 레이블 또는 이름을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-114">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="b38ce-115">다음 예제에서는 선택한 속성 "name" 및 "resourceGroup"에 "VMName" 및 "RGName" 레이블을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-115">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


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

## <a name="selecting-complex-nested-properties"></a><span data-ttu-id="b38ce-116">복잡한 중첩 속성 선택</span><span class="sxs-lookup"><span data-stu-id="b38ce-116">Selecting complex nested properties</span></span>

<span data-ttu-id="b38ce-117">선택하려는 속성이 JSON 출력 깊숙이 중첩된 경우 해당 중첩 속성의 전체 경로를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-117">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="b38ce-118">다음 예제에서는 vm 목록 명령에서 VMName 및 OS 유형을 선택하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-118">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

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

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="b38ce-119">contains 함수로 필터링</span><span class="sxs-lookup"><span data-stu-id="b38ce-119">Filter with the contains function</span></span>

<span data-ttu-id="b38ce-120">JMESPath `contains` 함수를 사용하여 쿼리에서 반환된 결과를 구체화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-120">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="b38ce-121">다음 예제의 명령은 이름에 "RGD"라는 텍스트가 포함된 VM만 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-121">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>  

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

<span data-ttu-id="b38ce-122">다음 예제의 결과는 vmSize 'Standard_DS1'이 포함된 VM을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-122">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

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

## <a name="filter-with-grep"></a><span data-ttu-id="b38ce-123">grep를 사용하여 필터링</span><span class="sxs-lookup"><span data-stu-id="b38ce-123">Filter with grep</span></span>

<span data-ttu-id="b38ce-124">`tsv` 출력 형식은 헤더 없이 탭으로 구분된 텍스트입니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-124">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="b38ce-125">`grep` 및 `cut` 같은 명령으로 전달하여 `list` 출력의 특정 값을 자세히 구문 분석할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-125">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="b38ce-126">다음 예제의 `grep` 명령은 이름에 "RGD"라는 텍스트가 포함된 VM만 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-126">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="b38ce-127">`cut` 명령은 8번째 필드(탭으로 구분됨) 값만 선택하여 출력에 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-127">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="b38ce-128">Jpterm을 사용하여 탐색</span><span class="sxs-lookup"><span data-stu-id="b38ce-128">Explore with jpterm</span></span>

<span data-ttu-id="b38ce-129">명령 출력을 [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal)로 전달하고 거기서 JMESPath 쿼리를 실험할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b38ce-129">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```


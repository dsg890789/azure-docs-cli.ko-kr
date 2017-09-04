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
ms.openlocfilehash: de37b1ad6aa55c9ac73b5b6b89d9507c86cc1245
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="93bca-104">Azure CLI 2.0 명령의 출력 형식</span><span class="sxs-lookup"><span data-stu-id="93bca-104">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="93bca-105">Azure CLI 2.0은 기본 출력 옵션으로 json을 사용하지만 모든 명령의 출력 형식을 지정하는 다양한 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-105">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="93bca-106">`--output`(또는 `--out` 또는 `-o`) 매개 변수를 사용하여 명령의 출력을 다음 테이블에 나와 있는 출력 형식 중 하나로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-106">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table.</span></span> 

<span data-ttu-id="93bca-107">--output</span><span class="sxs-lookup"><span data-stu-id="93bca-107">--output</span></span> | <span data-ttu-id="93bca-108">설명</span><span class="sxs-lookup"><span data-stu-id="93bca-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="93bca-109">json 문자열입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-109">json string.</span></span> <span data-ttu-id="93bca-110">기본값은 `json`입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-110">`json` is the default.</span></span>
`jsonc`  | <span data-ttu-id="93bca-111">색으로 구분된 json 문자열입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-111">colorized json string.</span></span>
`table`  | <span data-ttu-id="93bca-112">열 머리글이 있는 테이블입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-112">table with column headings.</span></span>
`tsv`    | <span data-ttu-id="93bca-113">탭으로 구분된 값입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-113">tab-separated values.</span></span>

## <a name="using-the-json-option"></a><span data-ttu-id="93bca-114">Json 옵션 사용</span><span class="sxs-lookup"><span data-stu-id="93bca-114">Using the json option</span></span>

<span data-ttu-id="93bca-115">다음 예제에서는 구독의 가상 컴퓨터 목록을 기본 json 형식으로 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-115">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli
az vm list --output json
```

<span data-ttu-id="93bca-116">결과는 이 형식(간단하게 표시하기 위해 출력의 일부만 표시)입니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-116">The results are in this form (only showing partial output for sake of brevity).</span></span>

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
 
## <a name="using-the-table-option"></a><span data-ttu-id="93bca-117">테이블 옵션 사용</span><span class="sxs-lookup"><span data-stu-id="93bca-117">Using the table option</span></span>

<span data-ttu-id="93bca-118">테이블 옵션은 읽기 쉬운 출력 집합을 제공하지만, 이전의 json 예제와는 달리 중첩된 개체는 단순 `--output table`을 사용하는 출력에 포함되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-118">The table option provides an easy to read set of output, but note that nested objects are not included in the output with the simple `--output table`, unlike the preceding .json example.</span></span>  <span data-ttu-id="93bca-119">'테이블' 출력 형식의 동일한 예제를 사용하면 가장 일반적인 속성 값 큐 레이트 목록이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-119">Using the same example with 'table' output format provides a curated list of most common property values.</span></span>

```azurecli
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

<span data-ttu-id="93bca-120">`--query` 매개 변수를 사용하여 목록 출력에 표시할 속성과 열을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="93bca-121">다음 예제에서는 `list` 명령에서 VM 이름 및 리소스 그룹 이름만 선택하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli
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

## <a name="using-the-tsv-option"></a><span data-ttu-id="93bca-122">tsv 옵션 사용</span><span class="sxs-lookup"><span data-stu-id="93bca-122">Using the tsv option</span></span>

<span data-ttu-id="93bca-123">'tsv' 출력 형식은 머리글과 대시 없이 간단한 텍스트 기반의 탭으로 구분된 출력을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-123">'tsv' output format returns a simple text-based and tab-separated output with no headings and dashes.</span></span> <span data-ttu-id="93bca-124">이 형식은 출력을 어떤 형태의 텍스트를 처리해야 하는 다른 명령 및 도구에 간편하게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-124">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="93bca-125">앞의 예제에 `tsv` 옵션을 사용하면 탭으로 구분된 결과가 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-125">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="93bca-126">다음 예제에서는 `tsv` 출력을 `grep` 및 `cut` 같은 명령으로 전달하여 `list` 출력의 특정 값을 자세히 구문 분석하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-126">The next example shows how the `tsv` output can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="93bca-127">`grep` 명령은 이름에 "RGD"라는 텍스트가 포함된 항목만 선택하고, `cut` 명령은 8번째 필드(탭으로 구분됨) 값만 선택하여 출력에 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-127">The `grep` command selects only items that have text "RGD" in them and then the `cut` command selects only the eighth field (separated by tabs) value to show in the output.</span></span>

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a><span data-ttu-id="93bca-128">기본 출력 형식 설정</span><span class="sxs-lookup"><span data-stu-id="93bca-128">Setting the default output format</span></span>

<span data-ttu-id="93bca-129">`az configure` 명령을 사용하여 환경을 설정하거나 출력 형식에 대한 기본 설정과 같은 기본 설정을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-129">You can use the `az configure` command to set up your environment or establish preferences such as default settings for output formats.</span></span> <span data-ttu-id="93bca-130">일반적인 예로, 가장 간단한 출력 형식 기본값은 "테이블" 형식입니다. 출력 형식을 선택하라는 메시지가 표시되면 **3**을 선택하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="93bca-130">For common use, the easiest output format default is the "table" format - select **3** when prompted for output format choices.</span></span> 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```
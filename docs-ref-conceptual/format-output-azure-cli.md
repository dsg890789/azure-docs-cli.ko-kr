---
title: Azure CLI 2.0의 출력 형식
description: Azure CLI 2.0 명령 출력을 테이블, 목록 또는 json 형식으로 지정하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 016465080e95af3ab0650146e955dd8cffc569e8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34305981"
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="94e1e-103">Azure CLI 2.0 명령의 출력 형식</span><span class="sxs-lookup"><span data-stu-id="94e1e-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="94e1e-104">Azure CLI 2.0은 기본 출력 옵션으로 json을 사용하지만 모든 명령의 출력 형식을 지정하는 다양한 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="94e1e-105">`--output`(또는 `--out` 또는 `-o`) 매개 변수를 사용하여 명령의 출력을 다음 테이블에 나와 있는 출력 형식 중 하나로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="94e1e-106">--output</span><span class="sxs-lookup"><span data-stu-id="94e1e-106">--output</span></span> | <span data-ttu-id="94e1e-107">설명</span><span class="sxs-lookup"><span data-stu-id="94e1e-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="94e1e-108">JSON 문자열</span><span class="sxs-lookup"><span data-stu-id="94e1e-108">JSON string.</span></span> <span data-ttu-id="94e1e-109">이 설정은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="94e1e-110">색으로 구분된 JSON</span><span class="sxs-lookup"><span data-stu-id="94e1e-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="94e1e-111">열 제목인 키가 포함된 ASCII 테이블</span><span class="sxs-lookup"><span data-stu-id="94e1e-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="94e1e-112">키가 포함되지 않은 탭으로 구분된 값</span><span class="sxs-lookup"><span data-stu-id="94e1e-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="94e1e-113">JSON 출력 형식</span><span class="sxs-lookup"><span data-stu-id="94e1e-113">JSON output format</span></span>

<span data-ttu-id="94e1e-114">다음 예제에서는 구독의 가상 머신 목록을 기본 json 형식으로 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="94e1e-115">다음과 같은 출력에는 편의를 위해 생략되고, 교체된 정보를 식별하는 몇몇 필드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="94e1e-116">테이블 출력 형식</span><span class="sxs-lookup"><span data-stu-id="94e1e-116">Table output format</span></span>

<span data-ttu-id="94e1e-117">`table` 출력 형식은 정렬된 데이터의 행과 열로 서식이 지정된 일반 출력을 제공하여 쉽게 읽고 검사할 수 있게 합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="94e1e-118">중첩된 개체는 테이블 출력에 포함되지 않지만 쿼리의 일부로 필터링될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="94e1e-119">일부 필드는 데이터에서 생략됩니다. 따라서 빠르고 검색 가능한 데이터의 개요를 만들려는 경우 이 형식을 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="94e1e-120">`--query` 매개 변수를 사용하여 목록 출력에 표시할 속성과 열을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="94e1e-121">다음 예제에서는 `list` 명령에서 VM 이름 및 리소스 그룹 이름만 선택하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="94e1e-122">특정 키는 필터링되고 테이블 보기에 인쇄되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="94e1e-123">`id`, `type` 및 `etag`가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="94e1e-124">출력에 표시해야 하는 경우 JMESPath 리키잉 기능을 사용하여 키 이름을 변경하고 필터링을 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="94e1e-125">데이터를 필터링하는 쿼리를 사용하는 방법에 대한 자세한 내용은 [Azure CLI 2.0과 함께 JMESPath 쿼리 사용](/cli/azure/query-azure-cli)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="94e1e-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="94e1e-126">TSV 출력 형식</span><span class="sxs-lookup"><span data-stu-id="94e1e-126">TSV output format</span></span>

<span data-ttu-id="94e1e-127">`tsv` 출력 형식은 추가 서식 지정, 키 또는 다른 기호 없이 탭 및 줄 바꿈으로 구분된 값을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="94e1e-128">이 형식은 출력을 어떤 형태의 텍스트를 처리해야 하는 다른 명령 및 도구에 간편하게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="94e1e-129">`table` 형식과 마찬가지로 `tsv` 출력 옵션은 중첩된 개체를 인쇄하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="94e1e-130">앞의 예제에 `tsv` 옵션을 사용하면 탭으로 구분된 결과가 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="94e1e-131">다음 예제에서는 `tsv` 출력을 UNIX 시스템의 다른 명령에 파이프하여 보다 구체적인 데이터를 추출할 수 있는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="94e1e-132">`grep` 명령은 이름에 "RGD"라는 텍스트가 포함된 항목을 선택하고, `cut` 명령은 8번째 필드(탭으로 구분됨)를 선택하여 출력에 VM 이름을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="94e1e-133">값은 탭으로 구분된 필드를 처리할 용도로 인쇄된 JSON 개체에 표시되는 것과 동일한 순서입니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="94e1e-134">이 순서는 명령에서 일관되게 실행되도록 보장됩니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="94e1e-135">기본 출력 형식을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-135">Set the default output format</span></span>

<span data-ttu-id="94e1e-136">대화형 `az configure` 명령을 사용하여 환경을 설정하고 출력 형식에 대한 기본 설정을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="94e1e-137">기본 출력 형식은 `json`입니다.</span><span class="sxs-lookup"><span data-stu-id="94e1e-137">The default output format is `json`.</span></span> 

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

<span data-ttu-id="94e1e-138">환경을 구성하는 방법에 대해 자세히 알아보려면 [Azure CLI 2.0 구성](/cli/azure/azure-cli-configuration)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="94e1e-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>
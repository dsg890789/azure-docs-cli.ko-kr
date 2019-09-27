---
title: Azure CLI의 출력 형식
description: Azure CLI 명령 출력을 테이블, 목록 또는 json 형식으로 지정하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/23/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 125055eec956e56c95af9a1c24ee4254e77556e6
ms.sourcegitcommit: 5b9b4446c08b94256ced7f63c145b493ba8b50df
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/24/2019
ms.locfileid: "71217442"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="9aa02-103">Azure CLI 명령의 출력 형식</span><span class="sxs-lookup"><span data-stu-id="9aa02-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="9aa02-104">Azure CLI는 기본 출력 형식으로 JSON을 사용하지만 다른 형식도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="9aa02-105">`--output`(`--out` 또는 `-o`) 매개 변수를 사용하여 CLI 출력의 형식을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="9aa02-106">인수 값과 출력의 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-106">The argument values and types of output are:</span></span>

<span data-ttu-id="9aa02-107">--output</span><span class="sxs-lookup"><span data-stu-id="9aa02-107">--output</span></span> | <span data-ttu-id="9aa02-108">설명</span><span class="sxs-lookup"><span data-stu-id="9aa02-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="9aa02-109">JSON 문자열</span><span class="sxs-lookup"><span data-stu-id="9aa02-109">JSON string.</span></span> <span data-ttu-id="9aa02-110">이 설정은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="9aa02-111">색으로 구분된 JSON</span><span class="sxs-lookup"><span data-stu-id="9aa02-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="9aa02-112">머신이 읽을 수 있는 JSON 대안인 YAML.</span><span class="sxs-lookup"><span data-stu-id="9aa02-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="9aa02-113">열 제목인 키가 포함된 ASCII 테이블</span><span class="sxs-lookup"><span data-stu-id="9aa02-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="9aa02-114">키가 포함되지 않은 탭으로 구분된 값</span><span class="sxs-lookup"><span data-stu-id="9aa02-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="9aa02-115">JSON 출력 형식</span><span class="sxs-lookup"><span data-stu-id="9aa02-115">JSON output format</span></span>

<span data-ttu-id="9aa02-116">다음 예제에서는 구독에 있는 가상 머신의 목록을 기본 JSON 형식으로 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-116">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="9aa02-117">다음과 같은 출력에는 편의를 위해 생략되고, 교체된 정보를 식별하는 몇몇 필드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="9aa02-118">YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="9aa02-118">YAML output format</span></span>

<span data-ttu-id="9aa02-119">`yaml` 형식은 출력을 일반 텍스트 데이터 serialization 형식인 [YAML](http://yaml.org/)로 인쇄합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="9aa02-120">YAML은 JSON보다 읽기 쉬우며, 해당 형식으로 쉽게 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="9aa02-121">일부 애플리케이션 및 CLI 명령은 JSON 대신 YAML을 구성 입력으로 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="9aa02-122">다음과 같은 출력에는 편의를 위해 생략되고, 교체된 정보를 식별하는 몇몇 필드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="9aa02-123">테이블 출력 형식</span><span class="sxs-lookup"><span data-stu-id="9aa02-123">Table output format</span></span>

<span data-ttu-id="9aa02-124">`table` 형식은 ASCII 테이블로 출력을 인쇄하여 읽고 검사하기 쉽게 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="9aa02-125">중첩된 개체는 테이블 출력에 포함되지 않지만 쿼리의 일부로 필터링될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="9aa02-126">일부 필드는 테이블에 포함되지 않습니다. 따라서 빠르고 검색 가능한 데이터의 개요를 만들려는 경우 이 형식을 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="9aa02-127">`--query` 매개 변수를 사용하여 목록 출력에 표시할 속성과 열을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="9aa02-128">다음 예제에서는 `list` 명령에서 VM 이름 및 리소스 그룹 이름만 선택하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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
> <span data-ttu-id="9aa02-129">일부 키는 기본적으로 테이블 보기에 인쇄되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="9aa02-130">`id`, `type` 및 `etag`가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="9aa02-131">출력에 표시해야 하는 경우 JMESPath 리키잉 기능을 사용하여 키 이름을 변경하고 필터링을 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="9aa02-132">데이터를 필터링하는 쿼리를 사용하는 방법에 대한 자세한 내용은 [Azure CLI와 함께 JMESPath 쿼리 사용](/cli/azure/query-azure-cli)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9aa02-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="9aa02-133">TSV 출력 형식</span><span class="sxs-lookup"><span data-stu-id="9aa02-133">TSV output format</span></span>

<span data-ttu-id="9aa02-134">`tsv` 출력 형식은 추가 서식 지정, 키 또는 다른 기호 없이 탭 및 줄 바꿈으로 구분된 값을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="9aa02-135">이 형식은 출력을 어떤 형태의 텍스트를 처리해야 하는 다른 명령 및 도구에 간편하게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="9aa02-136">`table` 형식과 마찬가지로 `tsv`는 중첩된 개체를 인쇄하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="9aa02-137">앞의 예제에 `tsv` 옵션을 사용하면 탭으로 구분된 결과가 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="9aa02-138">TSV 출력 형식의 제한 중 하나는 출력 순서에 대한 보장이 없다는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-138">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="9aa02-139">CLI는 순서를 유지하기 위해 응답 JSON의 키를 알파벳 순서로 정렬한 다음, TSV 출력을 위해 키 값을 인쇄합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-139">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="9aa02-140">하지만 Azure 서비스 응답 형식이 변경될 수 있으므로 순서가 항상 동일하다는 보장은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-140">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="9aa02-141">일관적인 순서를 적용하려면 `--query` 매개 변수와 [다중 선택 목록](query-azure-cli.md#get-multiple-values) 형식을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-141">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="9aa02-142">CLI 명령에서 단일 JSON 사전을 반환하는 경우 일반 형식 `[key1, key2, ..., keyN]`을 사용하여 키 순서를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-142">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="9aa02-143">배열을 반환하는 CLI 명령의 경우 일반 형식 `[].[key1, key2, ..., keyN]`을 사용하여 열 값의 순서를 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-143">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="9aa02-144">예를 들어 위에 표시되는 정보를 ID, 위치, 리소스 그룹 및 VM 이름순으로 지정하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-144">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

<span data-ttu-id="9aa02-145">다음 예제는 `tsv` 출력이 bash에서 다른 명령에 파이프되는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-145">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="9aa02-146">쿼리는 출력을 필터링하고 순서를 적용하는 데 사용되고, `grep`은 이름에 "RGD"라는 텍스트가 포함된 항목을 선택하고, `cut` 명령은 네 번째 필드를 선택하여 출력에 VM 이름을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-146">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="9aa02-147">기본 출력 형식을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-147">Set the default output format</span></span>

<span data-ttu-id="9aa02-148">대화형 `az configure` 명령을 사용하여 환경을 설정하고 출력 형식에 대한 기본 설정을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-148">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="9aa02-149">기본 출력 형식은 `json`입니다.</span><span class="sxs-lookup"><span data-stu-id="9aa02-149">The default output format is `json`.</span></span>

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
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

<span data-ttu-id="9aa02-150">환경을 구성하는 방법에 대해 자세히 알아보려면 [Azure CLI 구성](/cli/azure/azure-cli-configuration)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9aa02-150">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

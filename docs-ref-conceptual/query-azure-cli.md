---
title: Azure CLI를 사용한 쿼리 명령 결과
description: Azure CLI 명령의 출력에 대해 JMESPath 쿼리를 수행하는 방법을 학습합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1736d1677fb6c7fc83a092493e8706c2d5edfccd
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222534"
---
# <a name="use-jmespath-queries-with-azure-cli"></a><span data-ttu-id="121ee-103">Azure CLI와 함께 JMESPath 쿼리 사용</span><span class="sxs-lookup"><span data-stu-id="121ee-103">Use JMESPath queries with Azure CLI</span></span> 

<span data-ttu-id="121ee-104">Azure CLI는 `--query` 인수를 사용하여 명령의 결과에 대해 [JMESPath 쿼리](http://jmespath.org)를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="121ee-105">JMESPath는 JSON의 쿼리 언어이며, CLI 출력의 데이터를 선택하고 표시하는 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="121ee-106">다른 표시 형식 전에 이러한 쿼리를 JSON 출력에서 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="121ee-107">`--query` 인수는 Azure CLI의 모든 명령에서 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="121ee-108">이 문서의 예제는 일반적인 사용 사례를 다루고 JMESPath 기능을 사용하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="121ee-109">사전 출력으로 작업</span><span class="sxs-lookup"><span data-stu-id="121ee-109">Work with dictionary output</span></span>

<span data-ttu-id="121ee-110">JSON 사전을 반환하는 명령을 해당 키 이름만으로 탐색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="121ee-111">키 경로는 `.` 문자를 구분 기호로 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="121ee-112">다음 예제에서는 Linux VM에 연결할 수 있도록 허용된 공용 SSH 키 목록을 끌어옵니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="121ee-113">여러 값을 정렬된 배열에 배치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="121ee-114">다음 예제에서는 OS 디스크의 이름 및 크기를 제공하는 Azure 이미지를 검색하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="121ee-115">출력에 키를 배치하는 경우 대체 사전 구문을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="121ee-116">사전 출력할 요소 선택 영역은 `{displayKey:keyPath, ...}` 형식을 사용하여 `keyPath` JMESPath 식으로 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="121ee-117">출력 값에서, 키/값 쌍은 `{displayKey: value}`(으)로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="121ee-118">다음 예제에서는 마지막 예제의 쿼리를 사용하고 출력에 키를 할당하여 더 명확하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="121ee-119">`table` 출력 형식으로 정보를 표시할 때 사전 표시는 열 헤더를 설정할 수 있게 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="121ee-120">출력 형식에 대한 자세한 내용은 [Azure CLI 명령에 대한 출력 형식](/cli/azure/format-output-azure-cli)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="121ee-120">For more information on output formats, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="121ee-121">특정 키는 필터링되고 테이블 보기에 인쇄되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="121ee-122">이러한 키는 `id`, `type` 및 `etag`입니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="121ee-123">이 정보를 표시해야 하는 경우 키 이름을 변경하고 필터링하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="121ee-124">목록 출력으로 작업</span><span class="sxs-lookup"><span data-stu-id="121ee-124">Work with list output</span></span>

<span data-ttu-id="121ee-125">하나 이상의 값을 반환할 수 있는 CLI 명령은 배열을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="121ee-126">배열 요소는 인덱스에 의해 액세스되며 매번 같은 순서로 반환되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="121ee-127">`[]` 연산자를 사용하여 평면화하여 한 번에 모든 배열 요소를 쿼리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="121ee-128">연산자는 배열 뒤에 또는 식의 첫 번째 요소로 위치합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="121ee-129">배열을 평면화하면 배열의 각 요소에 대해 다음 쿼리를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="121ee-130">다음 예제에서는 리소스 그룹의 각 VM에서 실행 중인 이름 및 OS를 인쇄합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

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

<span data-ttu-id="121ee-131">키 경로의 일부인 배열도 평면화될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="121ee-132">다음 쿼리는 VM이 연결된 NIC의 Azure 개체 ID를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="121ee-133">조건자를 사용하여 배열 출력 필터링</span><span class="sxs-lookup"><span data-stu-id="121ee-133">Filter array output with predicates</span></span>

<span data-ttu-id="121ee-134">JMESPath는 [필터링 식](http://jmespath.org/specification.html#filterexpressions)을 제공하여 표시된 데이터를 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="121ee-135">이러한 식은 [JMESPath 기본 제공 함수](http://jmespath.org/specification.html#built-in-functions)와 함께 결합되어 부분적으로 일치를 수행하거나 표준 형식으로 데이터를 조작할 경우에 특히 강력합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="121ee-136">필터 식은 배열 데이터에서만 작동하고 다른 상황에서 사용될 때 `null` 값을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="121ee-137">예를 들어 `vm list`와 같은 명령의 출력을 사용하고 필터링하여 특정 형식의 VM을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="121ee-138">다음 예제에서는 Windows VM만을 캡처하고 해당 이름을 인쇄하도록 VM 형식을 필터링하여 이전 항목으로 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="121ee-139">대화형으로 쿼리를 사용하여 실험</span><span class="sxs-lookup"><span data-stu-id="121ee-139">Experiment with queries interactively</span></span>

<span data-ttu-id="121ee-140">JMESPath 학습을 시작하기 위해 [JMESPath-터미널](https://github.com/jmespath/jmespath.terminal) Python 패키지는 쿼리를 실험할 수 있는 대화형 환경을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="121ee-141">데이터는 입력으로 파이프되며 프로그램 내 쿼리는 데이터 추출을 위해 작성되고 편집됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ee-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

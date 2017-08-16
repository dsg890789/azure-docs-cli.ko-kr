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
ms.openlocfilehash: de6a366b84efa5475fd6146ff29c32e32dfe4672
ms.sourcegitcommit: 1791991b82e6ce8ad4a050cab1695e0c93734e08
ms.contentlocale: ko-KR
ms.lasthandoff: 05/12/2017
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="39cbe-104">대화형 Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="39cbe-104">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="39cbe-105">`az interactive` 명령을 실행하여 대화형 모드에서 Azure CLI 2.0을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-105">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="39cbe-106">그러면 명령이 자동으로 완성되고, 명령 및 해당 매개 변수에 대한 설명과 명령 예제에 액세스할 수 있는 대화형 셸로 이동됩니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-106">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![대화형 모드](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="39cbe-108">여기서는 검은색 배경에서는 잘 보이지 않는 기본 스타일을 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-108">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="39cbe-109">계정에 아직 로그인하지 않은 경우 `login` 명령을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-109">If you're not already logged in to your account, use the `login` command to do that.</span></span>

## <a name="configure"></a><span data-ttu-id="39cbe-110">구성</span><span class="sxs-lookup"><span data-stu-id="39cbe-110">Configure</span></span>

<span data-ttu-id="39cbe-111">대화형 모드는 필요에 따라 명령 설명, 매개 변수 설명 및 명령 예제를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-111">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="39cbe-112">`F1` 키를 사용해서 설명 및 예제를 표시하거나 표시하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-112">You can turn descriptions and examples on or off using `F1`.</span></span>

![설명 및 예제](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="39cbe-114">`F2` 키를 사용하여 매개 변수 기본값을 표시하거나 표시하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-114">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![기본값](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="39cbe-116">`F3` 키는 일부 키 제스처를 표시하거나 숨깁니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-116">`F3` toggles the display of some key gestures.</span></span>

![제스처](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="39cbe-118">범위</span><span class="sxs-lookup"><span data-stu-id="39cbe-118">Scope</span></span>

<span data-ttu-id="39cbe-119">대화형 모드의 범위를 `vm` 또는 `vm image`와 같은 특정 명령 그룹으로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-119">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="39cbe-120">이렇게 하면 해당 범위에서 모든 명령이 해석됩니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-120">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="39cbe-121">해당 명령 그룹에서 모든 작업을 수행하려는 경우에는 이 방법이 간단합니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-121">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="39cbe-122">다음 명령을 입력하는 대신</span><span class="sxs-lookup"><span data-stu-id="39cbe-122">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="39cbe-123">vm 명령 그룹으로 범위를 지정하고 다음 명령을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-123">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="39cbe-124">하위 수준 명령 그룹으로도 범위를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-124">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="39cbe-125">`%%vm image`를 사용하여 `vm image`로 범위를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-125">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="39cbe-126">이 경우 이미 `vm`으로 범위를 지정했으므로 `%%image`를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-126">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="39cbe-127">이때 `%%..`를 사용하여 범위를 `vm`으로 다시 되돌리거나 `%%`만 사용해서 범위를 루트로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-127">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="39cbe-128">쿼리</span><span class="sxs-lookup"><span data-stu-id="39cbe-128">Query</span></span>

<span data-ttu-id="39cbe-129">실행한 마지막 명령의 결과에 대해 JMESPath 쿼리를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-129">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="39cbe-130">예를 들어 VM을 만든 후 완전히 프로비전되었는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-130">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

<span data-ttu-id="39cbe-131">명령의 결과를 쿼리하는 방법에 대한 자세한 내용은 [Azure 2.0의 명령 결과 쿼리](query-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="39cbe-131">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="39cbe-132">Bash 명령</span><span class="sxs-lookup"><span data-stu-id="39cbe-132">Bash commands</span></span>

<span data-ttu-id="39cbe-133">`#[cmd]` 명령을 사용하여 대화형 모드를 종료하지 않고 셸 명령을 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="39cbe-134">예</span><span class="sxs-lookup"><span data-stu-id="39cbe-134">Examples</span></span>

<span data-ttu-id="39cbe-135">일부 명령에는 많은 예제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="39cbe-136">`CTRL-N`을 사용하여 예제의 다음 페이지로 스크롤하거나, `CTRL-Y`를 사용하여 예제의 이전 페이지로 스크롤할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![예제](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="39cbe-138">`::#`을 사용하여 구체적인 예제를 살펴볼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39cbe-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```

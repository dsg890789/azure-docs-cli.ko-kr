---
title: Azure CLI 대화형 모드
description: 대화형 모드에서 Azure CLI를 사용합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a325b799c7384037ae336093aa5274c7cbf53cbc
ms.sourcegitcommit: 334a1da92a73e42e715e33470057f4194f10b2ea
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/17/2019
ms.locfileid: "59429016"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="a690d-103">Azure CLI 대화형 모드</span><span class="sxs-lookup"><span data-stu-id="a690d-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="a690d-104">`az interactive` 명령을 실행하여 대화형 모드에서 Azure CLI 를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="a690d-105">이 모드는 자동 완성, 명령 설명 및 예제를 사용하는 대화형 셸을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![대화형 모드](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="a690d-107">여기서는 검은색 배경에서는 잘 보이지 않는 기본 스타일을 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="a690d-108">계정에 아직 로그인하지 않은 경우 `login` 명령을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="a690d-109">구성</span><span class="sxs-lookup"><span data-stu-id="a690d-109">Configure</span></span>

<span data-ttu-id="a690d-110">대화형 모드는 필요에 따라 명령 설명, 매개 변수 설명 및 명령 예제를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="a690d-111">`F1` 키를 사용해서 설명 및 예제를 표시하거나 표시하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-111">Turn descriptions and examples on or off using `F1`.</span></span>

![설명 및 예제](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="a690d-113">`F2` 키를 사용하여 매개 변수 기본값을 표시하거나 표시하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![기본값](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="a690d-115">`F3` 키는 일부 키 제스처를 표시하거나 숨깁니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-115">`F3` toggles the display of some key gestures.</span></span>

![제스처](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="a690d-117">범위</span><span class="sxs-lookup"><span data-stu-id="a690d-117">Scope</span></span>

<span data-ttu-id="a690d-118">대화형 모드의 범위를 `vm` 또는 `vm image`와 같은 특정 명령 그룹으로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="a690d-119">이렇게 하면 해당 범위에서 모든 명령이 해석됩니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="a690d-120">해당 명령 그룹에서 모든 작업을 수행하려는 경우에는 이 방법이 간단합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="a690d-121">다음 명령을 입력하는 대신</span><span class="sxs-lookup"><span data-stu-id="a690d-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="a690d-122">vm 명령 그룹으로 범위를 지정하고 다음 명령을 입력할 수 잇습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="a690d-123">하위 수준 명령 그룹으로도 범위를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="a690d-124">`%%vm image`를 사용하여 `vm image`로 범위를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="a690d-125">이 경우 이미 `vm`으로 범위를 지정했으므로 `%%image`를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="a690d-126">이때 `%%..`를 사용하여 범위를 `vm`으로 다시 되돌리거나 `%%`만 사용해서 범위를 루트로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="a690d-127">쿼리</span><span class="sxs-lookup"><span data-stu-id="a690d-127">Query</span></span>

<span data-ttu-id="a690d-128">`??` 다음에 JMESPath 쿼리를 사용하여 실행한 마지막 명령의 결과에 대해 JMESPath 쿼리를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-128">You can execute a JMESPath query on the results of the last command that you executed by using `??`followed by a JMESPath query.</span></span>
<span data-ttu-id="a690d-129">예를 들어 그룹을 만든 후 새 그룹의 ID를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-129">For example, after you created a group, you can retrieve the id of the new group.</span></span>

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

<span data-ttu-id="a690d-130">또한 이 구문을 사용하여 이전 명령의 결과를 다음 명령에 대한 인수로 사용할 수도 있습니다.\*
예를 들어 모든 그룹을 나열한 후 해당 위치가 서유럽인 첫 번째 그룹에 대해 형식 `virtualMachine`의 모든 리소스를 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-130">You can also use this syntax to use the result of the previous command as an argument for your next command.\* For instance after having listed all groups, list all the resources of type `virtualMachine`on the first group whose location is westeurope.</span></span> 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

<span data-ttu-id="a690d-131">명령의 결과를 쿼리하는 방법에 대한 자세한 내용은 [Azure CLI를 사용한 쿼리 명령 결과](query-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a690d-131">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="a690d-132">Bash 명령</span><span class="sxs-lookup"><span data-stu-id="a690d-132">Bash commands</span></span>

<span data-ttu-id="a690d-133">`#[cmd]` 명령을 사용하여 대화형 모드를 종료하지 않고 셸 명령을 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="a690d-134">예</span><span class="sxs-lookup"><span data-stu-id="a690d-134">Examples</span></span>

<span data-ttu-id="a690d-135">일부 명령에는 많은 예제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="a690d-136">`CTRL-N`을 사용하여 예제의 다음 페이지로 스크롤하거나, `CTRL-Y`를 사용하여 예제의 이전 페이지로 스크롤할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![예제](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="a690d-138">`::#`을 사용하여 구체적인 예제를 살펴볼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```

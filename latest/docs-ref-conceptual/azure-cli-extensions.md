---
title: "Azure CLI 2.0 확장"
description: "Azure CLI 2.0 확장 사용"
keywords: "Azure CLI, 확장"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a76e58c4430a184d133cca0ef0623f325aeb2f27
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="af5e6-104">Azure CLI 2.0 확장 사용</span><span class="sxs-lookup"><span data-stu-id="af5e6-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="af5e6-105">확장은 새 명령을 통해 기능을 추가할 수 있는 Azure CLI 자체와 함께 제공되지 않는 개별 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-105">Extensions are individual modules not shipped with the Azure CLI itself that allow you to add functionality through new commands.</span></span> <span data-ttu-id="af5e6-106">이러한 모듈은 실험적 또는 시험판 제품, Microsoft에서 사용자의 요구에 맞춘 특수 도구 또는 사용자가 직접 작성한 확장일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-106">These might be experimental or pre-release offerings, specialized tools that Microsoft has for your needs, or even extensions that you yourself have written.</span></span> <span data-ttu-id="af5e6-107">확장을 사용하면 CLI를 통해 유연성을 갖출 수 있으므로 핵심 기능 집합의 일부로 간주되지 않는 많은 추가 패키지를 제공하지 않고도 자신의 요구 사항에 맞게 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="af5e6-108">이 문서는 CLI 확장을 설치, 업데이트 및 제거하는 방법을 이해하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-108">This article will help you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="af5e6-109">또한 확장 동작에 대한 일반적인 질문에 대답하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="af5e6-110">확장 찾기</span><span class="sxs-lookup"><span data-stu-id="af5e6-110">Finding extensions</span></span>

<span data-ttu-id="af5e6-111">`az extension list-available`을 사용하면 사용 가능한 확장을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-111">In order to know what extensions are available, you can use `az extension list-available`.</span></span> <span data-ttu-id="af5e6-112">이 명령은 Microsoft에서 제공하고 지원하는 사용 가능한 공식 확장을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="af5e6-113">확장 설치</span><span class="sxs-lookup"><span data-stu-id="af5e6-113">Installing extensions</span></span>

<span data-ttu-id="af5e6-114">설치할 확장을 찾았으면 `az extension add`을 사용하여 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-114">Once you have found an extension to install, use `az extension add` to get it.</span></span> <span data-ttu-id="af5e6-115">확장이 `az extension list-available`에 나열된 공식 Microsoft 확장인 경우 확장을 이름별로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-115">If the extension is an official Microsoft extension listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="af5e6-116">확장이 외부 리소스에 있거나 직접 연결되는 링크가 있는 경우 원본 URL 또는 로컬 경로를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="af5e6-117">이는 _컴파일된 Python 휠 파일이어야 합니다_.</span><span class="sxs-lookup"><span data-stu-id="af5e6-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="af5e6-118">확장이 설치되었으면 `$AZURE_EXTENSION_DIR` 셸 변수 값에서 이 파일을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="af5e6-119">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="af5e6-120">확장 업데이트</span><span class="sxs-lookup"><span data-stu-id="af5e6-120">Updating extensions</span></span>

<span data-ttu-id="af5e6-121">확장은 이름별로만 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-121">Extensions can only be updated by name:</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="af5e6-122">어떤 이유로든 CLI에서 확장 이름을 확인할 수 없으면 확장을 다시 설치하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="af5e6-123">확장이 미리 보기에서 CLI의 기본 명령으로 전환되었을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="af5e6-124">이 경우 CLI를 업데이트하고 확장을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="af5e6-125">확장 제거</span><span class="sxs-lookup"><span data-stu-id="af5e6-125">Uninstalling extensions</span></span>

<span data-ttu-id="af5e6-126">확장이 더 이상 필요하지 않으면 `az extension remove`를 사용하여 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-126">If you no longer need an extension, it can be removed with `az extension remove`,</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="af5e6-127">확장을 설치한 위치에서 수동으로 삭제하여 제거할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="af5e6-128">이는 `$AZURE_EXTENSION_DIR` 셸 변수의 값입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="af5e6-129">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="af5e6-130">`az extension remove`를 사용하여 제거하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="af5e6-131">FAQ</span><span class="sxs-lookup"><span data-stu-id="af5e6-131">FAQ</span></span>

<span data-ttu-id="af5e6-132">다음은 CLI 확장에 대한 몇 가지 다른 일반적인 질문에 대한 답변입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="af5e6-133">설치에 사용할 수 있는 파일 형식은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="af5e6-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="af5e6-134">현재 컴파일된 Python 휠 파일만 확장으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="af5e6-135">확장에서 기존 명령을 바꿀 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="af5e6-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="af5e6-136">예.</span><span class="sxs-lookup"><span data-stu-id="af5e6-136">Yes.</span></span> <span data-ttu-id="af5e6-137">확장에서 기존 명령을 바꿀 수 있지만, 바꾼 명령이 실행되기 전에 CLI에서 경고가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="af5e6-138">확장이 시험판인지 어떻게 알 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="af5e6-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="af5e6-139">확장이 시험판인 경우 자체 설명서 및 버전 관리를 통해 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="af5e6-140">또한 Microsoft에서 일반적으로 제품을 미리 보기에서 기본 CLI 인터페이스로 전환하는 계획을 통해 CLI에 대한 미리 보기 명령을 확장으로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="af5e6-141">확장은 서로 종속될 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="af5e6-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="af5e6-142">아니요.</span><span class="sxs-lookup"><span data-stu-id="af5e6-142">No.</span></span> <span data-ttu-id="af5e6-143">확장은 각각 독립적인 개별 패키지입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="af5e6-144">이는 CLI에서 확장이 로드되는 시기를 보장하지 않으므로 종속성이 충족되지 못할 수 있기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="af5e6-145">확장을 설치하는 경우 해당 확장만 설치되며 다른 확장을 제거하더라도 계속 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="af5e6-146">확장은 CLI와 함께 업데이트되나요?</span><span class="sxs-lookup"><span data-stu-id="af5e6-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="af5e6-147">아니요.</span><span class="sxs-lookup"><span data-stu-id="af5e6-147">No.</span></span> <span data-ttu-id="af5e6-148">[확장 업데이트](#updating-extensions) 섹션에서 설명한 대로 확장은 별도로 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="af5e6-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>

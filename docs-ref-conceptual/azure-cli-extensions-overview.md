---
title: Azure CLI 2.0 확장
description: Azure CLI 2.0 확장 사용
keywords: Azure CLI, 확장
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a150edbc174ff77f4320a2cb60e031dc3c6ad1cc
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="018da-104">Azure CLI 2.0 확장 사용</span><span class="sxs-lookup"><span data-stu-id="018da-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="018da-105">확장은 Azure CLI 자체와 함께 제공되지 않는 새로운 명령을 통해 기능을 추가하는 개별 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="018da-106">이러한 확장은 Microsoft에서 제공하는 전문 도구 또는 사용자가 직접 작성하는 사용자 지정 기능과 같은 실험적인 기능 또는 릴리스 전 기능으로 제공될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="018da-107">확장을 사용하면 CLI를 통해 유연성을 갖출 수 있으므로 핵심 기능 집합의 일부로 간주되지 않는 많은 추가 패키지를 제공하지 않고도 자신의 요구 사항에 맞게 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="018da-108">이 문서에서는 CLI에 대한 확장을 설치, 업데이트 및 제거하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="018da-109">또한 확장 동작에 대한 일반적인 질문에 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="018da-110">확장 찾기</span><span class="sxs-lookup"><span data-stu-id="018da-110">Find extensions</span></span>

<span data-ttu-id="018da-111">[az extension list-available](/cli/azure/extension#az-extension-list-available)을 사용하면 사용할 수 있는 확장을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="018da-112">이 명령은 Microsoft에서 제공하고 관리하는 공식 확장 프로그램을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli
az extension list-available --output table
```

<span data-ttu-id="018da-113">설명서 사이트에도 [ Microsoft 확장 목록 ](azure-cli-extensions-list.md)이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="018da-114">확장 설치</span><span class="sxs-lookup"><span data-stu-id="018da-114">Install extensions</span></span>

<span data-ttu-id="018da-115">설치할 확장을 찾은 다음에는 [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-add)를 사용하여 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="018da-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="018da-116">확장이 `az extension list-available`에 나열된 경우 해당 이름으로 확장을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="018da-117">확장이 외부 리소스에 있거나 직접 연결되는 링크가 있는 경우 원본 URL 또는 로컬 경로를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="018da-118">이는 _컴파일된 Python 휠 파일이어야 합니다_.</span><span class="sxs-lookup"><span data-stu-id="018da-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="018da-119">확장이 설치되었으면 `$AZURE_EXTENSION_DIR` 셸 변수 값에서 이 파일을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="018da-120">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="018da-121">확장 업데이트</span><span class="sxs-lookup"><span data-stu-id="018da-121">Update extensions</span></span>

<span data-ttu-id="018da-122">확장이 이름별로 설치된 경우 [az 확장 업데이트](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-update)를 사용하여 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="018da-123">그렇지 않으면 [설치 확장](#install-extensions) 지침에 따라 소스에서 확장을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="018da-124">CLI가 확장 이름을 해석할 수 없는 경우 이를 제거하고 다시 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="018da-125">확장이 미리 보기에서 CLI의 기본 명령으로 전환되었을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="018da-126">[Azure CLI 2.0 설치](install-azure-cli.md)에 설명된 대로 CLI를 업데이트하고 확장 프로그램의 명령이 추가되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="018da-127">확장 제거</span><span class="sxs-lookup"><span data-stu-id="018da-127">Uninstall extensions</span></span>

<span data-ttu-id="018da-128">확장이 더 이상 필요하지 않으면 [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-remove)를 사용하여 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-remove).</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="018da-129">확장을 설치한 위치에서 수동으로 삭제하여 제거할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="018da-130">이는 `$AZURE_EXTENSION_DIR` 셸 변수의 값입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="018da-131">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="018da-132">`az extension remove`를 사용하여 제거하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="018da-133">FAQ</span><span class="sxs-lookup"><span data-stu-id="018da-133">FAQ</span></span>

<span data-ttu-id="018da-134">다음은 CLI 확장에 대한 몇 가지 다른 일반적인 질문에 대한 답변입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="018da-135">설치에 사용할 수 있는 파일 형식은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="018da-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="018da-136">현재 컴파일된 Python 휠 파일만 확장으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="018da-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="018da-137">확장에서 기존 명령을 바꿀 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="018da-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="018da-138">예.</span><span class="sxs-lookup"><span data-stu-id="018da-138">Yes.</span></span> <span data-ttu-id="018da-139">확장에서 기존 명령을 바꿀 수 있지만, 바꾼 명령이 실행되기 전에 CLI에서 경고가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="018da-140">확장이 시험판인지 어떻게 알 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="018da-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="018da-141">확장이 시험판인 경우 자체 설명서 및 버전 관리를 통해 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="018da-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="018da-142">또한 Microsoft에서 일반적으로 제품을 미리 보기에서 기본 CLI 인터페이스로 전환하는 계획을 통해 CLI에 대한 미리 보기 명령을 확장으로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="018da-143">확장은 서로 종속될 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="018da-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="018da-144">번호</span><span class="sxs-lookup"><span data-stu-id="018da-144">No.</span></span> <span data-ttu-id="018da-145">확장은 각각 독립적인 개별 패키지입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="018da-146">이는 CLI에서 확장이 로드되는 시기를 보장하지 않으므로 종속성이 충족되지 못할 수 있기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="018da-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="018da-147">확장을 설치하는 경우 해당 확장만 설치되며 다른 확장을 제거하더라도 계속 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="018da-148">확장은 CLI와 함께 업데이트되나요?</span><span class="sxs-lookup"><span data-stu-id="018da-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="018da-149">번호</span><span class="sxs-lookup"><span data-stu-id="018da-149">No.</span></span> <span data-ttu-id="018da-150">[확장 업데이트](#update-extensions)에 설명된 대로 확장은 별도로 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="018da-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

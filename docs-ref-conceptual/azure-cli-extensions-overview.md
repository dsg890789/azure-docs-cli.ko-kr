---
title: Azure CLI 확장
description: Azure CLI 확장 사용
keywords: Azure CLI, 확장
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4f203f94e9b26e1219bfe69ec0ddd73228d30b64
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593271"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="9b7e3-104">Azure CLI 확장 사용</span><span class="sxs-lookup"><span data-stu-id="9b7e3-104">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="9b7e3-105">Azure CLI는 확장을 로드하는 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-105">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="9b7e3-106">확장은 Python 휠로, CLI의 일부로 함께 제공되지 않지만 CLI 명령으로 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-106">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="9b7e3-107">확장 기능을 사용하면 자체 CLI 인터페이스를 작성하는 기능과 함께 시험 및 시험판 명령에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-107">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="9b7e3-108">이 문서에서는 확장을 관리하는 방법을 설명하고 해당 사용에 대한 일반적인 질문에 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-108">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="9b7e3-109">확장 찾기</span><span class="sxs-lookup"><span data-stu-id="9b7e3-109">Find extensions</span></span>

<span data-ttu-id="9b7e3-110">Microsoft에서 제공 및 유지 관리하는 확장을 참조하려면, [az extension list-available](/cli/azure/extension#az-extension-list-available) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-110">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="9b7e3-111">설명서 사이트에 [확장 목록](azure-cli-extensions-list.md)도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-111">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="9b7e3-112">확장 설치</span><span class="sxs-lookup"><span data-stu-id="9b7e3-112">Install extensions</span></span>

<span data-ttu-id="9b7e3-113">설치할 확장을 찾은 다음에는 [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add)를 사용하여 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-113">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="9b7e3-114">확장이 `az extension list-available`에 나열된 경우 해당 이름으로 확장을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="9b7e3-115">확장이 외부 리소스에 있거나 직접 연결되는 링크가 있는 경우 원본 URL 또는 로컬 경로를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="9b7e3-116">이 확장은 _컴파일된 Python 휠 파일이어야 합니다_.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="9b7e3-117">확장이 설치되었으면 `$AZURE_EXTENSION_DIR` 셸 변수 값에서 이 파일을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="9b7e3-118">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="9b7e3-119">확장 업데이트</span><span class="sxs-lookup"><span data-stu-id="9b7e3-119">Update extensions</span></span>

<span data-ttu-id="9b7e3-120">확장이 이름별로 설치된 경우 [az 확장 업데이트](https://docs.microsoft.com/cli/azure/extension#az-extension-update)를 사용하여 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-120">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="9b7e3-121">그렇지 않으면 [설치 확장](#install-extensions) 지침에 따라 소스에서 확장을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-121">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="9b7e3-122">CLI가 확장 이름을 해석할 수 없는 경우 이를 제거하고 다시 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-122">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="9b7e3-123">확장은 기본 CLI의 일부가 되었을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-123">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="9b7e3-124">[Azure CLI 설치](install-azure-cli.md)에 설명된 대로 CLI를 업데이트하고 확장 프로그램의 명령이 추가되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-124">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="9b7e3-125">확장 제거</span><span class="sxs-lookup"><span data-stu-id="9b7e3-125">Uninstall extensions</span></span>

<span data-ttu-id="9b7e3-126">확장이 더 이상 필요하지 않으면 [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove)를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-126">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="9b7e3-127">확장을 설치한 위치에서 수동으로 삭제하여 제거할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="9b7e3-128">`$AZURE_EXTENSION_DIR` 셸 변수는 모듈 설치 위치를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-128">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="9b7e3-129">이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="9b7e3-130">FAQ</span><span class="sxs-lookup"><span data-stu-id="9b7e3-130">FAQ</span></span>

<span data-ttu-id="9b7e3-131">다음은 CLI 확장에 대한 몇 가지 다른 일반적인 질문에 대한 답변입니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-131">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="9b7e3-132">설치에 사용할 수 있는 파일 형식은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="9b7e3-132">What file formats are allowed for installation?</span></span>

<span data-ttu-id="9b7e3-133">현재 컴파일된 Python 휠 파일만 확장으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-133">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="9b7e3-134">확장에서 기존 명령을 바꿀 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="9b7e3-134">Can extensions replace existing commands?</span></span>

<span data-ttu-id="9b7e3-135">예.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-135">Yes.</span></span> <span data-ttu-id="9b7e3-136">확장에서 기존 명령을 바꿀 수 있지만, 바꾼 명령이 실행되기 전에 CLI에서 경고가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-136">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="9b7e3-137">확장이 시험판인지 어떻게 알 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="9b7e3-137">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="9b7e3-138">시험판인 경우 확장의 설명서 및 버전 관리가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-138">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="9b7e3-139">Microsoft는 종종 CLI 확장으로 미리보기 명령을 출시하고, 나중에 메인 CLI 제품으로 옮길 수 있는 옵션을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-139">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="9b7e3-140">명령이 확장 외부로 이동되면, 이전 확장을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-140">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="9b7e3-141">확장은 서로 종속될 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="9b7e3-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="9b7e3-142"> 아니요.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-142">No.</span></span> <span data-ttu-id="9b7e3-143">CLI는 로드 순서를 보장하지 않으므로 종속성을 충족하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-143">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="9b7e3-144">확장을 제거하는 것은 다른 것에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-144">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="9b7e3-145">확장은 CLI와 함께 업데이트되나요?</span><span class="sxs-lookup"><span data-stu-id="9b7e3-145">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="9b7e3-146"> 아니요.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-146">No.</span></span> <span data-ttu-id="9b7e3-147">[확장 업데이트](#update-extensions)에 설명된 대로 확장은 별도로 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9b7e3-147">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

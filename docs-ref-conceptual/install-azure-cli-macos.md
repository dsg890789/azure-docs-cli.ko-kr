---
title: "macOS용 Azure CLI 설치"
description: "macOS에 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure macos, azure 설치 macos"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="c8cc6-104">macOS에 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="c8cc6-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="c8cc6-105">macOS 플랫폼의 경우 [homebrew 패키지 관리자](http://brew.sh)를 통해 또는 수동으로 Azure CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="c8cc6-106">필요할 때 간편하게 설치, 업데이트 및 제거할 수 있도록 기본 설치 방법으로 homebrew가 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="c8cc6-107">homebrew를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="c8cc6-107">Use homebrew to install</span></span>

<span data-ttu-id="c8cc6-108">Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="c8cc6-109">설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="c8cc6-110">`apt` 또는 `yum` 같은 다른 패키지 관리자와 비슷합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="c8cc6-111">시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="c8cc6-112">homebrew로 설치</span><span class="sxs-lookup"><span data-stu-id="c8cc6-112">Install with homebrew</span></span>

<span data-ttu-id="c8cc6-113">brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="c8cc6-114">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="c8cc6-115">homebrew로 업데이트</span><span class="sxs-lookup"><span data-stu-id="c8cc6-115">Update with homebrew</span></span>

<span data-ttu-id="c8cc6-116">CLI는 버그 픽스, 향상된 기능, 새로운 기능 및 미리 보기 기능이 정기적으로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="c8cc6-117">약 2주마다 새 릴리스가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="c8cc6-118">로컬 리포지토리 정보를 업데이트한 후 CLI 패키지를 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="c8cc6-119">문제 해결</span><span class="sxs-lookup"><span data-stu-id="c8cc6-119">Troubleshooting</span></span>

<span data-ttu-id="c8cc6-120">homebrew를 사용하여 CLI를 설치 또는 업데이트할 때 문제가 발생했습니까?</span><span class="sxs-lookup"><span data-stu-id="c8cc6-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="c8cc6-121">다음은 발생할 수 있는 몇 가지 일반적인 오류와 그 진단 및 해결 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="c8cc6-122">Python 또는 설치된 패키지를 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="c8cc6-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="c8cc6-123">설치에서 Python 또는 설치된 패키지를 찾을 수 없는 경우 부 버전 불일치 또는 homebrew 설치 과정에서 다른 문제가 있는 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="c8cc6-124">CLI는 virtualenv를 사용하지 않으므로 homebrew가 올바른 Python 버전을 찾는 것에 의존합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="c8cc6-125">Python 설치를 다시 연결하면 이러한 문제가 해결될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="c8cc6-126">CLI 버전 만료</span><span class="sxs-lookup"><span data-stu-id="c8cc6-126">The CLI version is out of date</span></span>

<span data-ttu-id="c8cc6-127">설치된 CLI 버전이 만료된 것일 수도 있다는 생각이 들면 `brew update` 명령, `brew upgrade azure-cli` 명령을 차례로 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="c8cc6-128">이 방법으로도 CLI가 업데이트되지 않는 경우 homebrew 패키지는 일반 릴리스보다 더 늦게 출시될 수 있다는 점에 주의하세요.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="c8cc6-129">CLI의 첨단 설치가 필요한 경우 [수동으로 설치](#manage-the-cli-manually)해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="c8cc6-130">Homebrew로 제거</span><span class="sxs-lookup"><span data-stu-id="c8cc6-130">Uninstall with homebrew</span></span>

<span data-ttu-id="c8cc6-131">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="c8cc6-132">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="c8cc6-133">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="c8cc6-134">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="c8cc6-135">homebrew로 설치한 경우 제거 시에도 homebrew를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="c8cc6-136">CLI 수동 설치</span><span class="sxs-lookup"><span data-stu-id="c8cc6-136">Install the CLI manually</span></span>

<span data-ttu-id="c8cc6-137">homebrew를 사용하여 CLI 설치를 자동으로 관리할 수 없거나 하고 싶지 않은 경우 수동으로 설치하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="c8cc6-138">[Linux 수동 설치 지침](install-azure-cli-linux.md)에 따라 macOS에 수동으로 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="c8cc6-139">macOS 10.9 이상 버전에는 필요한 모든 종속성이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8cc6-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>

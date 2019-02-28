---
title: macOS용 Azure CLI 설치
description: macOS에 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 61be6c31e7251c8b374bf09072a9ecba9b914342
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422054"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="6073f-103">macOS에 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="6073f-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="6073f-104">macOS 플랫폼의 경우 [homebrew 패키지 관리자](https://brew.sh)를 사용하여 Azure CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="6073f-105">Homebrew를 사용하면 손쉽게 CLI 업데이트 설치를 최신으로 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="6073f-106">CLI 패키지는 macOS 버전 10.9 이상에서 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install"></a><span data-ttu-id="6073f-107">설치</span><span class="sxs-lookup"><span data-stu-id="6073f-107">Install</span></span>

<span data-ttu-id="6073f-108">Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="6073f-109">설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="6073f-110">시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.</span><span class="sxs-lookup"><span data-stu-id="6073f-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="6073f-111">brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="6073f-112">Azure CLI는 Homebrew의 `python3` 패키지에 종속되어 있으므로 Python 2를 사용할 수 있는 경우에도 시스템에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-112">The Azure CLI has a dependency on the `python3` package in Homebrew, and will install it on your system, even if Python 2 is available.</span></span> <span data-ttu-id="6073f-113">Azure CLI는 Homebrew에 게시된 최신 버전의 `python3`과 호환되도록 보장됩니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="6073f-114">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6073f-115">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6073f-116">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6073f-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6073f-117">문제 해결</span><span class="sxs-lookup"><span data-stu-id="6073f-117">Troubleshooting</span></span>

<span data-ttu-id="6073f-118">Homebrew 통해 CLI를 설치하는 경우 문제가 발생하는 경우 몇 가지 공용 오류가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="6073f-119">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6073f-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="6073f-120">Python 또는 설치된 패키지를 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="6073f-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="6073f-121">homebrew 설치 중 사소한 버전 불일치 또는 다른 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="6073f-122">CLI는 Python 가상 환경을 사용하지 않으므로, 설치된 Python 버전을 찾는 것에 의존합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="6073f-123">가능한 수정 방법은 프로그램을 설치하고 Homebrew에서 `python3` 종속성을 다시 연결하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="6073f-124">CLI 버전 1.x가 설치되었습니다</span><span class="sxs-lookup"><span data-stu-id="6073f-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="6073f-125">낮은 버전이 설치된 경우 부실한 homebrew 캐시로 인한 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="6073f-126">[업데이트](#Update) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="6073f-126">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="6073f-127">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="6073f-127">Update</span></span>

<span data-ttu-id="6073f-128">CLI는 버그 픽스, 향상된 기능, 새로운 기능 및 미리 보기 기능이 정기적으로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-128">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="6073f-129">약 2주마다 새 릴리스가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-129">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="6073f-130">로컬 리포지토리 정보를 업데이트한 후 `azure-cli` 패키지를 업그레이드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-130">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6073f-131">제거</span><span class="sxs-lookup"><span data-stu-id="6073f-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6073f-132">Homebrew를 사용하여 `azure-cli` 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-132">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="6073f-133">다른 설치 방법</span><span class="sxs-lookup"><span data-stu-id="6073f-133">Other installation methods</span></span>

<span data-ttu-id="6073f-134">Homebrew를 사용하여 사용자 환경에 Azure CLI를 설치할 수 없는 경우 Linux용 설명서 지침을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-134">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="6073f-135">이 프로세스는 공식적으로 macOS와 호환되도록 유지되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-135">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="6073f-136">Homebrew와 같은 패키지 관리자를 사용하는 것이 항상 권장됩니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-136">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="6073f-137">사용할 수 있는 다른 옵션이 없는 경우에만 수동 설치 방법을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6073f-137">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="6073f-138">수동 설치 지침은 [Linux에 Azure CLI 수동 설치](install-azure-cli-linux.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6073f-138">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6073f-139">다음 단계</span><span class="sxs-lookup"><span data-stu-id="6073f-139">Next Steps</span></span>

<span data-ttu-id="6073f-140">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="6073f-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6073f-141">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="6073f-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

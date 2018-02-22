---
title: "macOS용 Azure CLI 설치"
description: "macOS에 Azure CLI 2.0을 설치하는 방법"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0295846abc2fe6091940824c6efc47b8fd64ce9f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="156e2-103">macOS에 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="156e2-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="156e2-104">macOS 플랫폼의 경우 [homebrew 패키지 관리자](http://brew.sh)를 사용하여 Azure CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="156e2-105">Homebrew를 사용하면 손쉽게 CLI 업데이트 설치를 최신으로 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="156e2-106">CLI 패키지는 macOS 버전 10.9 이상에서 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="156e2-107">설치</span><span class="sxs-lookup"><span data-stu-id="156e2-107">Install</span></span>

<span data-ttu-id="156e2-108">Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="156e2-109">설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="156e2-110">시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.</span><span class="sxs-lookup"><span data-stu-id="156e2-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="156e2-111">brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="156e2-112">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-112">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="156e2-113">문제 해결</span><span class="sxs-lookup"><span data-stu-id="156e2-113">Troubleshooting</span></span>

<span data-ttu-id="156e2-114">Homebrew 통해 CLI를 설치하는 경우 문제가 발생하는 경우 몇 가지 공용 오류가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-114">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="156e2-115">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="156e2-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="156e2-116">Python 또는 설치된 패키지를 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="156e2-116">Unable to find Python or installed packages</span></span>

<span data-ttu-id="156e2-117">설치에서 Python 또는 설치된 패키지를 찾을 수 없는 경우 부 버전 불일치 또는 homebrew 설치 과정에서 발생한 다른 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-117">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="156e2-118">CLI는 Python 가상환경을 사용하지 않으므로 올바른 Python 버전을 찾는 것에 의존합니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-118">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="156e2-119">Python 설치를 다시 연결하면 이러한 문제가 해결될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-119">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="156e2-120">CLI 버전 1.x가 설치되었습니다</span><span class="sxs-lookup"><span data-stu-id="156e2-120">CLI version 1.x is installed</span></span>

<span data-ttu-id="156e2-121">낮은 버전이 설치된 경우 부실한 homebrew 캐시로 인한 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-121">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="156e2-122">[업데이트](#Update) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="156e2-122">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="156e2-123">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="156e2-123">Update</span></span>

<span data-ttu-id="156e2-124">CLI는 버그 픽스, 향상된 기능, 새로운 기능 및 미리 보기 기능이 정기적으로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-124">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="156e2-125">약 2주마다 새 릴리스가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-125">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="156e2-126">로컬 리포지토리 정보를 업데이트한 후 `azure-cli` 패키지를 업그레이드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-126">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="156e2-127">제거</span><span class="sxs-lookup"><span data-stu-id="156e2-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="156e2-128">Homebrew를 사용하여 `azure-cli` 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="156e2-128">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

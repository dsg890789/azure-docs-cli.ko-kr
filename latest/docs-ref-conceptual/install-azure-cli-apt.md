---
title: "apt를 사용하여 Azure CLI 2.0 설치"
description: "apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure apt, azure debian, azure ubuntu"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 93d947d91973def1c05e2f5b2e7511bc1c5704a2
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="35a8e-104">apt를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="35a8e-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="35a8e-105">Ubuntu 또는 Debian처럼 `apt`와 함께 제공되는 배포를 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="35a8e-106">CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="35a8e-107">배포에 패키지가 없으면 [Python](https://www.python.org/downloads/)을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="35a8e-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="35a8e-108">설치</span><span class="sxs-lookup"><span data-stu-id="35a8e-108">Install</span></span>

1. <span data-ttu-id="35a8e-109">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-109">Modify your sources list:</span></span>
 
   - <span data-ttu-id="35a8e-110">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="35a8e-110">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="35a8e-111">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="35a8e-111">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="35a8e-112">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-112">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="35a8e-113">`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-113">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="35a8e-114">업데이트</span><span class="sxs-lookup"><span data-stu-id="35a8e-114">Update</span></span>

<span data-ttu-id="35a8e-115">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-115">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="35a8e-116">이렇게 하면 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-116">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="35a8e-117">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="35a8e-117">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="35a8e-118">제거</span><span class="sxs-lookup"><span data-stu-id="35a8e-118">Uninstall</span></span>

<span data-ttu-id="35a8e-119">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-119">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="35a8e-120">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-120">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="35a8e-121">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-121">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="35a8e-122">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-122">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="35a8e-123">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-123">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="35a8e-124">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-124">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="35a8e-125">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="35a8e-125">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

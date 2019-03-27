---
title: apt를 사용하여 Linux에 Azure CLI 설치
description: apt 패키지 관리자를 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343148"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="89bde-103">apt를 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="89bde-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="89bde-104">Ubuntu 또는 Debian과 같이 `apt`와 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 x86_64 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="89bde-105">이 패키지는 다음 항목에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-105">This package has been tested with:</span></span>

* <span data-ttu-id="89bde-106">Ubuntu trusty, xenial, artful 및 bionic</span><span class="sxs-lookup"><span data-stu-id="89bde-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="89bde-107">Debian wheezy, jessie 및 stretch</span><span class="sxs-lookup"><span data-stu-id="89bde-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="89bde-108">Azure CLI용 패키지는 자체 Python 인터프리터를 설치하고 시스템 Python을 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="89bde-109">설치</span><span class="sxs-lookup"><span data-stu-id="89bde-109">Install</span></span>

1. <span data-ttu-id="89bde-110">설치 프로세스에 필요한 패키지를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-110">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. <span data-ttu-id="89bde-111">Microsoft 서명 키를 다운로드하고 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-111">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="89bde-112">Azure CLI 소프트웨어 리포지토리를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-112">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="89bde-113">리포지토리 정보를 업데이트하고 `azure-cli` 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-113">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="89bde-114">`az` 명령을 사용하여 Azure CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-114">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="89bde-115">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-115">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="89bde-116">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="89bde-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="89bde-117">문제 해결</span><span class="sxs-lookup"><span data-stu-id="89bde-117">Troubleshooting</span></span>

<span data-ttu-id="89bde-118">`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="89bde-119">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="89bde-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="89bde-120">lsb_release가 올바른 기본 배포 버전을 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="89bde-121">Linux Mint 같은 일부 Ubuntu 또는 Debian 파생 배포판은 `lsb_release`로부터 올바른 버전 이름을 반환하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="89bde-122">이 값은 설치 과정에서 패키지 설치를 확인하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="89bde-123">배포본이 파생된 Ubuntu 또는 Debian 버전의 코드 이름을 알고 있다면 [리포지토리를 추가](#set-release)할 때 수동으로 `AZ_REPO` 값을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-123">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="89bde-124">그렇지 않은 경우 귀하의 배포에 대해 기본 배포 코드 이름을 확인하고 `AZ_REPO`를 올바른 값으로 설정 하는 방법에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-124">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="89bde-125">배포에 필요한 패키지가 없음</span><span class="sxs-lookup"><span data-stu-id="89bde-125">No package for your distribution</span></span>

<span data-ttu-id="89bde-126">배포본이 릴리스된 후에 Azure CLI 패키지가 제공되기까지는 어느 정도 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-126">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="89bde-127">Azure CLI는 향후 버전의 종속성에 대해 탄력성을 갖도록 설계되었으며 가능한 한 적게 의존합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="89bde-128">기본 배포에 사용할 수 있는 패키지가 없는 경우 이전 배포 패키지를 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="89bde-129">이를 위해, [리포지토리를 추가](#set-release)할 때 수동으로 `AZ_REPO` 값을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-129">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="89bde-130">Ubuntu 배포의 경우 `bionic` 리포지토리를 사용하고 Debian 배포판의 경우 `stretch`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="89bde-131">Ubuntu Trusty 및 Debian Wheezy 이전에 릴리스된 배포는 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="89bde-132">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="89bde-132">Update</span></span>

<span data-ttu-id="89bde-133">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-133">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="89bde-134">이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-134">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="89bde-135">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="89bde-135">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="89bde-136">제거</span><span class="sxs-lookup"><span data-stu-id="89bde-136">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="89bde-137">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-137">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="89bde-138">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-138">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="89bde-139">서명 키를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-139">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="89bde-140">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="89bde-140">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="89bde-141">다음 단계</span><span class="sxs-lookup"><span data-stu-id="89bde-141">Next Steps</span></span>

<span data-ttu-id="89bde-142">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="89bde-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="89bde-143">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="89bde-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

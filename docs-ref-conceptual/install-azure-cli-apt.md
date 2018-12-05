---
title: apt를 사용하여 Linux에 Azure CLI 설치
description: apt 패키지 관리자를 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c33c3e75991979a72a7b82183dd88b87715907ae
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450261"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="1fa49-103">apt를 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="1fa49-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="1fa49-104">Ubuntu 또는 Debian과 같이 `apt`와 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 64비트 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="1fa49-105">이 패키지는 다음 항목에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-105">This package has been tested with:</span></span>

* <span data-ttu-id="1fa49-106">Ubuntu trusty, xenial, artful 및 bionic</span><span class="sxs-lookup"><span data-stu-id="1fa49-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="1fa49-107">Debian wheezy, jessie 및 stretch</span><span class="sxs-lookup"><span data-stu-id="1fa49-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="1fa49-108">설치</span><span class="sxs-lookup"><span data-stu-id="1fa49-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="1fa49-109">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="1fa49-110">Microsoft 서명 키 가져오기:</span><span class="sxs-lookup"><span data-stu-id="1fa49-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="1fa49-111">CLI 설치:</span><span class="sxs-lookup"><span data-stu-id="1fa49-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="1fa49-112">서명 키는 2018년 5월 업데이트되었으며 대체 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="1fa49-113">서명 오류가 발생할 경우 [최신 서명 키](#signingKey)가 있는 지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="1fa49-114">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1fa49-115">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1fa49-116">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1fa49-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1fa49-117">문제 해결</span><span class="sxs-lookup"><span data-stu-id="1fa49-117">Troubleshooting</span></span>

<span data-ttu-id="1fa49-118">`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="1fa49-119">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1fa49-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="1fa49-120">lsb_release가 올바른 기본 배포 버전을 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="1fa49-121">Linux Mint 같은 일부 Ubuntu 또는 Debian 파생 배포판은 `lsb_release`로부터 올바른 버전 이름을 반환하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="1fa49-122">이 값은 설치 과정에서 패키지 설치를 확인하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="1fa49-123">귀하의 배포가 파생된 출처 버전의 이름을 알고 있는 경우는 `AZ_REPO` 값을 수동으로 [1 단계 설치](#install-step-1)에 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="1fa49-124">그렇지 않은 경우 귀하의 배포에 대해 기본 배포 이름을 확인하고 `AZ_REPO`를 올바른 값으로 설정 하는 방법에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="1fa49-125">배포에 필요한 패키지가 없음</span><span class="sxs-lookup"><span data-stu-id="1fa49-125">No package for your distribution</span></span>

<span data-ttu-id="1fa49-126">Ubuntu 배포본이 릴리스된 후에 Azure CLI 패키지가 제공되기까지는 어느 정도 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-126">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="1fa49-127">Azure CLI는 향후 버전의 종속성에 대해 탄력성을 갖도록 설계되었으며 가능한 한 적게 의존합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="1fa49-128">기본 배포에 사용할 수 있는 패키지가 없는 경우 이전 배포 패키지를 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="1fa49-129">이를 위해 [1 단계 설치](#install-step-1)에서 `AZ_REPO`값을 수동으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-129">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="1fa49-130">Ubuntu 배포의 경우 `bionic` 리포지토리를 사용하고 Debian 배포판의 경우 `stretch`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="1fa49-131">Ubuntu Trusty 및 Debian Wheezy 이전에 릴리스된 배포는 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="1fa49-132">apt-key가 "dirmngr 없음"과 함께 실패</span><span class="sxs-lookup"><span data-stu-id="1fa49-132">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="1fa49-133">`apt-key` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-133">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="1fa49-134">이 오류는 `apt-key`에 필요한 구성 요소가 누락되었기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-134">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="1fa49-135">`dirmngr` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-135">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="1fa49-136">apt-key 중지</span><span class="sxs-lookup"><span data-stu-id="1fa49-136">apt-key hangs</span></span>

<span data-ttu-id="1fa49-137">포트 11371로 나가는 연결을 차단하는 방화벽 뒤에 있는 경우 `apt-key` 명령이 무기한 중지될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-137">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="1fa49-138">방화벽에 나가는 연결에 대한 HTTP 프록시가 필요할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-138">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="1fa49-139">프록시가 있는지 알아보려면, 시스템 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="1fa49-139">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="1fa49-140">프록시에 로그인이 필요하지 않으면 사용자와 암호 정보는 생략합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-140">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="1fa49-141">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="1fa49-141">Update</span></span>

<span data-ttu-id="1fa49-142">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="1fa49-143">서명 키는 2018년 5월 업데이트되었으며 대체 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-143">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="1fa49-144">서명 오류가 발생할 경우 [최신 서명 키](#signingKey)가 있는 지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-144">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="1fa49-145">이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-145">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="1fa49-146">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="1fa49-146">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="1fa49-147">제거</span><span class="sxs-lookup"><span data-stu-id="1fa49-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="1fa49-148">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-148">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="1fa49-149">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-149">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="1fa49-150">서명 키를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-150">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="1fa49-151">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1fa49-151">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="1fa49-152">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1fa49-152">Next Steps</span></span>

<span data-ttu-id="1fa49-153">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="1fa49-153">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1fa49-154">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="1fa49-154">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

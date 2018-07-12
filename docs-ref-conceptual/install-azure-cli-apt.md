---
title: apt를 사용하여 Linux에 Azure CLI 2.0 설치
description: apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/24/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3f52f1545dc4bad44280c7e58ad17ec2302fd436
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439621"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="6acbf-103">apt를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="6acbf-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="6acbf-104">Ubuntu 또는 Debian과 같이 `apt`과(와) 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 64비트 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="6acbf-105">이 패키지는 다음 항목에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-105">This package has been tested with:</span></span>

* <span data-ttu-id="6acbf-106">Ubuntu trusty, xenial, artful 및 bionic</span><span class="sxs-lookup"><span data-stu-id="6acbf-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="6acbf-107">Debian wheezy, jessie 및 stretch</span><span class="sxs-lookup"><span data-stu-id="6acbf-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="6acbf-108">설치</span><span class="sxs-lookup"><span data-stu-id="6acbf-108">Install</span></span>

1. <span data-ttu-id="6acbf-109"><a name="install-step-1"/>원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-109"><a name="install-step-1"/> Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <a name="signingKey"></a><span data-ttu-id="6acbf-110">Microsoft 서명 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="6acbf-111">CLI 설치:</span><span class="sxs-lookup"><span data-stu-id="6acbf-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="6acbf-112">서명 키는 2018년 5월 업데이트되었으며 대체 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="6acbf-113">서명 키 오류를 수신하는 경우 [최신 서명 키를 획득](#signingKey)했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="6acbf-114">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6acbf-115">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-115">To log in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6acbf-116">다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6acbf-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6acbf-117">문제 해결</span><span class="sxs-lookup"><span data-stu-id="6acbf-117">Troubleshooting</span></span>

<span data-ttu-id="6acbf-118">`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="6acbf-119">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6acbf-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="6acbf-120">lsb_release가 “명령을 찾을 수 없음”으로 인해 실패</span><span class="sxs-lookup"><span data-stu-id="6acbf-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="6acbf-121">`lsb_release` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="6acbf-122">이 오류는 lsb_release가 설치되어 있지 않기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="6acbf-123">`lsb-release` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="6acbf-124">lsb_release는 기본 배포 버전을 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="6acbf-125">Linux Mint 같은 일부 Ubuntu 또는 Debian 파생 배포판은 `lsb_release`로부터 올바른 버전 이름을 반환하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="6acbf-126">이 값은 설치 과정에서 패키지 설치를 확인하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="6acbf-127">귀하의 배포가 파생된 출처 버전의 이름을 알고 있는 경우는 `AZ_REPO` 값을 수동으로 [1 단계 설치](#install-step-1)에 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="6acbf-128">그렇지 않은 경우 귀하의 배포에 대해 기본 배포 이름을 확인하고 `AZ_REPO`를 올바른 값으로 설정 하는 방법에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="6acbf-129">apt-key가 "dirmngr 없음"과 함께 실패</span><span class="sxs-lookup"><span data-stu-id="6acbf-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="6acbf-130">`apt-key` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="6acbf-131">이 오류는 `apt-key`에 필요한 구성 요소가 누락되었기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="6acbf-132">`dirmngr` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="6acbf-133">apt-key 중지</span><span class="sxs-lookup"><span data-stu-id="6acbf-133">apt-key hangs</span></span>

<span data-ttu-id="6acbf-134">포트 11371로 나가는 연결을 차단하는 방화벽 뒤에 있는 경우 `apt-key` 명령이 무기한 중지될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="6acbf-135">방화벽은 나가는 연결을 위해 HTTP 프록시를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="6acbf-136">프록시가 있는지 여부를 모르는 경우 시스템 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="6acbf-136">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="6acbf-137">프록시에 로그인이 필요하지 않으면 사용자, 암호 및 `@` 토큰은 생략합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-137">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="6acbf-138">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="6acbf-138">Update</span></span>

<span data-ttu-id="6acbf-139">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="6acbf-140">서명 키는 2018년 5월 업데이트되었으며 대체 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="6acbf-141">서명 키 오류를 수신하는 경우 [최신 서명 키를 획득](#signingKey)했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
   
> [!NOTE]
> <span data-ttu-id="6acbf-142">이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="6acbf-143">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="6acbf-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="6acbf-144">제거</span><span class="sxs-lookup"><span data-stu-id="6acbf-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6acbf-145">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="6acbf-146">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-146">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="6acbf-147">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="6acbf-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

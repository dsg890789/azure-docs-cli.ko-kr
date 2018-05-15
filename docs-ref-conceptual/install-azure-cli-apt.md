---
title: apt를 사용하여 Linux에 Azure CLI 2.0 설치
description: apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7eb04b408f403264f3951bf663d43686601c4ab8
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/09/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="f52c2-103">apt를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="f52c2-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="f52c2-104">Ubuntu 또는 Debian과 같이 `apt`과(와) 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 64비트 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="f52c2-105">이 패키지는 다음 항목에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-105">This package has been tested with:</span></span>

* <span data-ttu-id="f52c2-106">Ubuntu trusty, xenial 및 artful</span><span class="sxs-lookup"><span data-stu-id="f52c2-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="f52c2-107">Debian wheezy, jessie 및 stretch</span><span class="sxs-lookup"><span data-stu-id="f52c2-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="f52c2-108">설치</span><span class="sxs-lookup"><span data-stu-id="f52c2-108">Install</span></span>

1. <span data-ttu-id="f52c2-109">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="f52c2-110">Microsoft 서명 키 가져오기:</span><span class="sxs-lookup"><span data-stu-id="f52c2-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="f52c2-111">이 서명 키는 사용되지 않으며 2018년 5월말 대체될 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="f52c2-112">`apt`를 사용하여 계속 업데이트하려면 새 키도 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="f52c2-113">CLI 설치:</span><span class="sxs-lookup"><span data-stu-id="f52c2-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="f52c2-114">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f52c2-115">로그인 하려면 `az login` 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="f52c2-116">다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f52c2-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f52c2-117">문제 해결</span><span class="sxs-lookup"><span data-stu-id="f52c2-117">Troubleshooting</span></span>

<span data-ttu-id="f52c2-118">`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="f52c2-119">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f52c2-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="f52c2-120">lsb_release가 “명령을 찾을 수 없음”으로 인해 실패</span><span class="sxs-lookup"><span data-stu-id="f52c2-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="f52c2-121">`lsb_release` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="f52c2-122">이 오류는 lsb_release가 설치되어 있지 않기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="f52c2-123">`lsb-release` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="f52c2-124">apt-key가 "dirmngr 없음"과 함께 실패</span><span class="sxs-lookup"><span data-stu-id="f52c2-124">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="f52c2-125">`apt-key` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-125">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="f52c2-126">이 오류는 `apt-key`에 필요한 구성 요소가 누락되었기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-126">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="f52c2-127">`dirmngr` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-127">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="f52c2-128">apt-key 중지</span><span class="sxs-lookup"><span data-stu-id="f52c2-128">apt-key hangs</span></span>

<span data-ttu-id="f52c2-129">포트 11371로 나가는 연결을 차단하는 방화벽 뒤에 있는 경우 `apt-key` 명령이 무기한 중지될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-129">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="f52c2-130">방화벽은 나가는 연결을 위해 HTTP 프록시를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-130">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="f52c2-131">프록시가 있는지 여부를 모르는 경우 시스템 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="f52c2-131">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="f52c2-132">프록시에 로그인이 필요하지 않으면 사용자, 암호 및 `@` 토큰은 생략합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-132">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="f52c2-133">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="f52c2-133">Update</span></span>

<span data-ttu-id="f52c2-134">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-134">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="f52c2-135">이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-135">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="f52c2-136">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="f52c2-136">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="f52c2-137">제거</span><span class="sxs-lookup"><span data-stu-id="f52c2-137">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="f52c2-138">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-138">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="f52c2-139">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-139">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="f52c2-140">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f52c2-140">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

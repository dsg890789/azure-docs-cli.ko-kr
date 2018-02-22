---
title: "apt를 사용하여 Linux에 Azure CLI 2.0 설치"
description: "apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4076fefb902a324f77f97bc042b9f5ba3e787734
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="c3d0b-103">apt를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="c3d0b-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="c3d0b-104">Ubuntu 또는 Debian과 같이 `apt`과(와) 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 64비트 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="c3d0b-105">이 패키지는 다음 항목에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-105">This package has been tested with:</span></span>

* <span data-ttu-id="c3d0b-106">Ubuntu wheezy, xenial 및 artful</span><span class="sxs-lookup"><span data-stu-id="c3d0b-106">Ubuntu wheezy, xenial, and artful</span></span>
* <span data-ttu-id="c3d0b-107">Debian wheezy, jessie 및 stretch</span><span class="sxs-lookup"><span data-stu-id="c3d0b-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="c3d0b-108">설치</span><span class="sxs-lookup"><span data-stu-id="c3d0b-108">Install</span></span>

1. <span data-ttu-id="c3d0b-109">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="c3d0b-110">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="c3d0b-111">`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c3d0b-112">문제 해결</span><span class="sxs-lookup"><span data-stu-id="c3d0b-112">Troubleshooting</span></span>

<span data-ttu-id="c3d0b-113">`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="c3d0b-114">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c3d0b-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="c3d0b-115">apt-key가 "dirmngr 없음"과 함께 실패</span><span class="sxs-lookup"><span data-stu-id="c3d0b-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="c3d0b-116">`apt-key` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="c3d0b-117">이 오류는 `apt-key`에 필요한 구성 요소가 누락되었기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="c3d0b-118">`dirmngr` 패키지를 설치하면 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="c3d0b-119">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="c3d0b-119">Update</span></span>

<span data-ttu-id="c3d0b-120">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-120">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="c3d0b-121">이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-121">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="c3d0b-122">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-122">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="c3d0b-123">제거</span><span class="sxs-lookup"><span data-stu-id="c3d0b-123">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="c3d0b-124">`apt-get remove`를 사용하여 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-124">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="c3d0b-125">CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-125">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="c3d0b-126">불필요한 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c3d0b-126">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

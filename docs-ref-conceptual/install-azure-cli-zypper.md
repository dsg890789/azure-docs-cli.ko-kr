---
title: zypper를 사용하여 Linux에 Azure CLI 설치
description: zypper를 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7e5897fe545527aa2708432e0ad0cf626584c785
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216884"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="1c454-103">zypper를 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="1c454-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="1c454-104">openSUSE 또는 SLES 등의 `zypper`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="1c454-105">이 패키지는 openSUSE Leap 15.1 및 SLES 15와 함께 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="1c454-106">설치</span><span class="sxs-lookup"><span data-stu-id="1c454-106">Install</span></span>

1. <span data-ttu-id="1c454-107">`curl` 설치:</span><span class="sxs-lookup"><span data-stu-id="1c454-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="1c454-108">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="1c454-109">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="1c454-110">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="1c454-111">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1c454-112">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1c454-113">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1c454-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1c454-114">문제 해결</span><span class="sxs-lookup"><span data-stu-id="1c454-114">Troubleshooting</span></span>

<span data-ttu-id="1c454-115">`zypper`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="1c454-116">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1c454-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-other-systems-without-python-36"></a><span data-ttu-id="1c454-117">Python 3.6 없이 SLES 12 또는 기타 시스템에 설치</span><span class="sxs-lookup"><span data-stu-id="1c454-117">Install on SLES 12 or other other systems without Python 3.6</span></span>

<span data-ttu-id="1c454-118">SLES 12에서 기본 python3 패키지는 3.4이며 Azure CLI에서 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-118">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="1c454-119">먼저 원본에서 더 높은 버전의 python3를 빌드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-119">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="1c454-120">그런 다음 Azure CLI 패키지를 다운로드하여 종속성 없이 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-120">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure --with-ssl
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="1c454-121">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="1c454-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="1c454-122">`yast2`를 통해 이 프록시를 항상 사용하도록 명시적으로 `zypper`를 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-122">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="1c454-123">이렇게 하려면 `yast2 proxy` 명령을 슈퍼 사용자 권한으로 실행하고 양식에 제공된 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-123">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="1c454-124">시스템에서 창 관리자를 사용할 수 있으면 `YaST Control Center`에서 `Network Services > Proxy` 창을 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-124">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="1c454-125">고급 구성 또는 자세한 내용은 [openSUSE 프록시 구성 설명서](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1c454-125">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="1c454-126">Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-126">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="1c454-127">업데이트</span><span class="sxs-lookup"><span data-stu-id="1c454-127">Update</span></span>

<span data-ttu-id="1c454-128">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-128">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="1c454-129">제거</span><span class="sxs-lookup"><span data-stu-id="1c454-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="1c454-130">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-130">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="1c454-131">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-131">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="1c454-132">다른 Microsoft 패키지를 사용하지 않는 경우 Microsoft 서명 키를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="1c454-132">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="1c454-133">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1c454-133">Next Steps</span></span>

<span data-ttu-id="1c454-134">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="1c454-134">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1c454-135">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="1c454-135">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

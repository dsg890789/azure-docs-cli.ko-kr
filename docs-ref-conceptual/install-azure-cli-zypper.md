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
ms.openlocfilehash: f8a3bec4fffb731c6521fa7b8a2a90798ef191e6
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516259"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="00b6c-103">zypper를 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="00b6c-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="00b6c-104">openSUSE 또는 SLES 등의 `zypper`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="00b6c-105">이 패키지는 openSUSE 42.2 이상 및 SLES 12 SP 2 이상에서 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-105">This package has been tested with openSUSE 42.2 and later, and SLES 12 SP 2 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="00b6c-106">설치</span><span class="sxs-lookup"><span data-stu-id="00b6c-106">Install</span></span>

1. <span data-ttu-id="00b6c-107">`curl` 설치:</span><span class="sxs-lookup"><span data-stu-id="00b6c-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="00b6c-108">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="00b6c-109">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="00b6c-110">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="00b6c-111">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="00b6c-112">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="00b6c-113">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="00b6c-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="00b6c-114">문제 해결</span><span class="sxs-lookup"><span data-stu-id="00b6c-114">Troubleshooting</span></span>

<span data-ttu-id="00b6c-115">`zypper`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="00b6c-116">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="00b6c-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="00b6c-117">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="00b6c-117">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="00b6c-118">`yast2`를 통해 이 프록시를 항상 사용하도록 명시적으로 `zypper`를 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-118">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="00b6c-119">이렇게 하려면 `yast2 proxy` 명령을 슈퍼 사용자 권한으로 실행하고 양식에 제공된 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-119">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="00b6c-120">시스템에서 창 관리자를 사용할 수 있으면 `YaST Control Center`에서 `Network Services > Proxy` 창을 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-120">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="00b6c-121">고급 구성 또는 자세한 내용은 [openSUSE 프록시 구성 설명서](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="00b6c-121">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="00b6c-122">Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-122">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="00b6c-123">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="00b6c-123">Update</span></span>

<span data-ttu-id="00b6c-124">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-124">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="00b6c-125">제거</span><span class="sxs-lookup"><span data-stu-id="00b6c-125">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="00b6c-126">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-126">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="00b6c-127">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-127">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="00b6c-128">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="00b6c-128">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="00b6c-129">다음 단계</span><span class="sxs-lookup"><span data-stu-id="00b6c-129">Next Steps</span></span>

<span data-ttu-id="00b6c-130">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="00b6c-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="00b6c-131">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="00b6c-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

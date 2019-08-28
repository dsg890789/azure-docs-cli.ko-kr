---
title: yum을 사용하여 Linux에 Azure CLI 설치
description: yum을 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bc3ae41ea04ae8d7f62242b2bfe415c8a3bfea33
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516291"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="bacfb-103">yum을 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="bacfb-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="bacfb-104">RHEL, Fedora, CentOS 등의 `yum`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="bacfb-105">이 패키지는 RHEL 7, Fedora 19 이상, CentOS 7를 사용하여 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="bacfb-106">설치</span><span class="sxs-lookup"><span data-stu-id="bacfb-106">Install</span></span>

1. <span data-ttu-id="bacfb-107">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="bacfb-108">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="bacfb-109">`yum install` 명령을 사용하여 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="bacfb-110">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="bacfb-111">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="bacfb-112">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bacfb-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="bacfb-113">문제 해결</span><span class="sxs-lookup"><span data-stu-id="bacfb-113">Troubleshooting</span></span>

<span data-ttu-id="bacfb-114">`yum`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="bacfb-115">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="bacfb-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="bacfb-116">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="bacfb-116">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="bacfb-117">이 프록시를 항상 사용하도록 명시적으로 `yum`을 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-117">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="bacfb-118">`/etc/yum.conf`의 `[main]` 섹션 아래에 다음 줄이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-118">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="bacfb-119">Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-119">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="bacfb-120">업데이트</span><span class="sxs-lookup"><span data-stu-id="bacfb-120">Update</span></span>

<span data-ttu-id="bacfb-121">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-121">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="bacfb-122">제거</span><span class="sxs-lookup"><span data-stu-id="bacfb-122">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="bacfb-123">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-123">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="bacfb-124">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-124">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="bacfb-125">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bacfb-125">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="bacfb-126">다음 단계</span><span class="sxs-lookup"><span data-stu-id="bacfb-126">Next Steps</span></span>

<span data-ttu-id="bacfb-127">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="bacfb-127">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="bacfb-128">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="bacfb-128">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

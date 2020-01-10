---
title: yum을 사용하여 Linux에 Azure CLI 설치
description: yum을 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f65240524942c2534f61b9cc51101812c8d09351
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216925"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="04026-103">yum을 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="04026-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="04026-104">RHEL, Fedora, CentOS 등의 `yum`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="04026-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="04026-105">이 패키지는 RHEL 7.7, RHEL 8, Fedora 24 이상, CentOS 7 및 CentOS 8에서 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="04026-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="04026-106">설치</span><span class="sxs-lookup"><span data-stu-id="04026-106">Install</span></span>

1. <span data-ttu-id="04026-107">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="04026-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="04026-108">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="04026-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="04026-109">`yum install` 명령을 사용하여 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="04026-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="04026-110">`az` 명령을 사용하여 Azure CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="04026-111">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="04026-112">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="04026-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="04026-113">문제 해결</span><span class="sxs-lookup"><span data-stu-id="04026-113">Troubleshooting</span></span>

<span data-ttu-id="04026-114">`yum`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="04026-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="04026-115">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="04026-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="04026-116">Python 3 없이 RHEL 7.6 또는 기타 시스템에 설치</span><span class="sxs-lookup"><span data-stu-id="04026-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="04026-117">가능하면 `python3` 패키지를 공식적으로 지원하는 버전으로 시스템을 업그레이드하십시오.</span><span class="sxs-lookup"><span data-stu-id="04026-117">If you can, please upgrade your system to a verison with official support for `python3` package.</span></span> <span data-ttu-id="04026-118">그렇지 않으면 먼저 [소스에서 빌드](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x)하거나 일부 [추가 리포지토리](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/)를 통해 `python3` 패키지를 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="04026-119">그런 다음 패키지를 다운로드하여 종속성 없이 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="04026-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="04026-120">가장 권장되지 않는 옵션은 Python 2를 계속 사용하면서 [수동 설치 지침](install-azure-cli-linux.md)을 따르는 것입니다. Python 2는 2020 년 1월 1일에 수명이 종료되기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="04026-120">The least recommended option is to still use Python 2 and follow the [manual install instructions](install-azure-cli-linux.md) since Python 2 is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="04026-121">향후 버전의 Azure CLI에서는 Python 2.7에 대한 지원이 중단됩니다.</span><span class="sxs-lookup"><span data-stu-id="04026-121">A future version of Azure CLI will drop support for Python 2.7.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="04026-122">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="04026-122">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="04026-123">이 프록시를 항상 사용하도록 명시적으로 `yum`를 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="04026-123">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="04026-124">`/etc/yum.conf`의 `[main]` 섹션 아래에 다음 줄이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-124">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="04026-125">Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-125">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="04026-126">업데이트</span><span class="sxs-lookup"><span data-stu-id="04026-126">Update</span></span>

<span data-ttu-id="04026-127">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-127">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="04026-128">제거</span><span class="sxs-lookup"><span data-stu-id="04026-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="04026-129">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-129">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="04026-130">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-130">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="04026-131">다른 Microsoft 패키지를 사용하지 않는 경우 서명 키를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="04026-131">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="04026-132">다음 단계</span><span class="sxs-lookup"><span data-stu-id="04026-132">Next Steps</span></span>

<span data-ttu-id="04026-133">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="04026-133">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="04026-134">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="04026-134">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

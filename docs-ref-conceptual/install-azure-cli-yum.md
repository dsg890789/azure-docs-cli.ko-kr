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
ms.devlang: azure-cli
ms.openlocfilehash: 3747f276a30740602271477e154322cad45f190e
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652467"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="cf13e-103">yum을 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="cf13e-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="cf13e-104">RHEL, Fedora, CentOS 등의 `yum`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="cf13e-105">이 패키지는 RHEL 7, Fedora 19 이상, CentOS 7를 사용하여 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="cf13e-106">설치</span><span class="sxs-lookup"><span data-stu-id="cf13e-106">Install</span></span>

1. <span data-ttu-id="cf13e-107">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="cf13e-108">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="cf13e-109">`yum install` 명령을 사용하여 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="cf13e-110">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="cf13e-111">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="cf13e-112">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cf13e-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="cf13e-113">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="cf13e-113">Update</span></span>

<span data-ttu-id="cf13e-114">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="cf13e-115">제거</span><span class="sxs-lookup"><span data-stu-id="cf13e-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="cf13e-116">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="cf13e-117">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-117">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="cf13e-118">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="cf13e-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="cf13e-119">다음 단계</span><span class="sxs-lookup"><span data-stu-id="cf13e-119">Next Steps</span></span>

<span data-ttu-id="cf13e-120">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="cf13e-120">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="cf13e-121">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="cf13e-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

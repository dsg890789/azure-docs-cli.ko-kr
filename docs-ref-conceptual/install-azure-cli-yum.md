---
title: yum을 사용하여 Linux에 Azure CLI 2.0 설치
description: yum을 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b3c82825af3d1d2420b0111d1a370a17f37d9426
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2018
ms.locfileid: "32043706"
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="871c1-103">yum을 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="871c1-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="871c1-104">RHEL, Fedora, CentOS 등의 `yum`과 함께 제공되는 배포를 실행하는 경우 Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="871c1-105">이 패키지는 RHEL 7, Fedora 19 이상, CentOS 7를 사용하여 테스트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="871c1-106">설치</span><span class="sxs-lookup"><span data-stu-id="871c1-106">Install</span></span>

1. <span data-ttu-id="871c1-107">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="871c1-108">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="871c1-109">`yum install` 명령을 사용하여 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="871c1-110">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="871c1-111">로그인 하려면 `az login` 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-111">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="871c1-112">다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="871c1-112">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="871c1-113">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="871c1-113">Update</span></span>

<span data-ttu-id="871c1-114">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="871c1-115">제거</span><span class="sxs-lookup"><span data-stu-id="871c1-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="871c1-116">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="871c1-117">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="871c1-118">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="871c1-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

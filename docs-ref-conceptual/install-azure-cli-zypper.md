---
title: zypper를 사용하여 Linux에 Azure CLI 2.0 설치
description: zypper를 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01d293eff229ab8b0eb3a3ff4e23978ea9e00174
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="dc1e2-103">zypper를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="dc1e2-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="dc1e2-104">openSUSE 또는 SLES 등의 `zypper`과 함께 제공되는 배포를 실행하는 경우 Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="dc1e2-105">이 패키지는 openSUSE 42.2 및 SLES 12 SP 2와 함께 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="dc1e2-106">설치</span><span class="sxs-lookup"><span data-stu-id="dc1e2-106">Install</span></span>

1. <span data-ttu-id="dc1e2-107">`curl` 설치:</span><span class="sxs-lookup"><span data-stu-id="dc1e2-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="dc1e2-108">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="dc1e2-109">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="dc1e2-110">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="dc1e2-111">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="dc1e2-112">로그인 하려면 `az login` 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="dc1e2-113">다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="dc1e2-114">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="dc1e2-114">Update</span></span>

<span data-ttu-id="dc1e2-115">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="dc1e2-116">제거</span><span class="sxs-lookup"><span data-stu-id="dc1e2-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="dc1e2-117">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="dc1e2-118">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="dc1e2-119">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dc1e2-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```


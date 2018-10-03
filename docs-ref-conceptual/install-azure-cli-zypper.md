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
ms.devlang: azure-cli
ms.openlocfilehash: 201cce81046d5039a313b918ac48b2849352995c
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177677"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="c5d4f-103">zypper를 사용하여 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="c5d4f-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="c5d4f-104">openSUSE 또는 SLES 등의 `zypper`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="c5d4f-105">이 패키지는 openSUSE 42.2 및 SLES 12 SP 2와 함께 테스트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="c5d4f-106">설치</span><span class="sxs-lookup"><span data-stu-id="c5d4f-106">Install</span></span>

1. <span data-ttu-id="c5d4f-107">`curl` 설치:</span><span class="sxs-lookup"><span data-stu-id="c5d4f-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="c5d4f-108">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="c5d4f-109">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="c5d4f-110">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="c5d4f-111">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c5d4f-112">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="c5d4f-113">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="c5d4f-114">주 지역에서</span><span class="sxs-lookup"><span data-stu-id="c5d4f-114">Update</span></span>

<span data-ttu-id="c5d4f-115">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="c5d4f-116">제거</span><span class="sxs-lookup"><span data-stu-id="c5d4f-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="c5d4f-117">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="c5d4f-118">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-118">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="c5d4f-119">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
## <a name="next-steps"></a><span data-ttu-id="c5d4f-120">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c5d4f-120">Next Steps</span></span>

<span data-ttu-id="c5d4f-121">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="c5d4f-121">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c5d4f-122">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="c5d4f-122">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

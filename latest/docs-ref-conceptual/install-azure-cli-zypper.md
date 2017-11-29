---
title: "zypper를 사용하여 Azure CLI 2.0 설치"
description: "zypper를 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "azure cli, azure cli 설치, azure cli zypper, azure cli opensuse, azure cli sle"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="dfc56-104">zypper를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="dfc56-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="dfc56-105">OpenSUSE 또는 SLE처럼 `zypper`와 함께 제공되는 배포를 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="dfc56-106">CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="dfc56-107">배포에 패키지가 없으면 [Python](https://www.python.org/downloads/)을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="dfc56-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="dfc56-108">설치</span><span class="sxs-lookup"><span data-stu-id="dfc56-108">Install</span></span> 

1. <span data-ttu-id="dfc56-109">`curl` 설치:</span><span class="sxs-lookup"><span data-stu-id="dfc56-109">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="dfc56-110">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-110">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="dfc56-111">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-111">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="dfc56-112">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-112">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="dfc56-113">`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-113">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="dfc56-114">업데이트</span><span class="sxs-lookup"><span data-stu-id="dfc56-114">Update</span></span>

<span data-ttu-id="dfc56-115">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="dfc56-116">제거</span><span class="sxs-lookup"><span data-stu-id="dfc56-116">Uninstall</span></span>

<span data-ttu-id="dfc56-117">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="dfc56-118">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="dfc56-119">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="dfc56-120">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="dfc56-121">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-121">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="dfc56-122">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-122">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="dfc56-123">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="dfc56-123">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```


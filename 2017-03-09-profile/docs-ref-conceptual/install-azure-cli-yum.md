---
title: "yum을 사용하여 Azure CLI 2.0 설치"
description: "yum을 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure yum,azure rhel, azure fedora, azure centos"
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
ms.openlocfilehash: de695454c6f3109679b9eb9f6c0d77348d354518
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="0e73a-104">yum을 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="0e73a-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="0e73a-105">RHEL, Fedora 또는 CentOS처럼 `yum`과 함께 제공되는 배포판을 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="0e73a-106">CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="0e73a-107">배포에 패키지가 없으면 [Python](https://www.python.org/downloads/)을 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="0e73a-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="0e73a-108">설치</span><span class="sxs-lookup"><span data-stu-id="0e73a-108">Install</span></span> 

1. <span data-ttu-id="0e73a-109">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-109">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="0e73a-110">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-110">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="0e73a-111">`yum` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-111">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="0e73a-112">`az` 명령을 사용하여 Azure CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-112">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="0e73a-113">업데이트</span><span class="sxs-lookup"><span data-stu-id="0e73a-113">Update</span></span>

<span data-ttu-id="0e73a-114">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="0e73a-115">제거</span><span class="sxs-lookup"><span data-stu-id="0e73a-115">Uninstall</span></span>

<span data-ttu-id="0e73a-116">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-116">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="0e73a-117">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-117">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="0e73a-118">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-118">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="0e73a-119">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-119">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="0e73a-120">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-120">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="0e73a-121">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-121">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="0e73a-122">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0e73a-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

---
title: Linux용 Azure CLI 2.0 수동 설치
description: Linux용 Azure CLI 2.0을 수동으로 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c5c7ea61a35e915760081897e88d8c43b80919e0
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388357"
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="a32f9-103">Linux에 Azure CLI 2.0 수동 설치</span><span class="sxs-lookup"><span data-stu-id="a32f9-103">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="a32f9-104">배포를 위한 Azure CLI용 패키지가 없다면 스크립트를 실행하여 수동으로 CLI를 설치하십시오.</span><span class="sxs-lookup"><span data-stu-id="a32f9-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

> [!NOTE]
> <span data-ttu-id="a32f9-105">패키지 관리자를 사용하여 CLI를 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="a32f9-106">패키지 관리자가 항상 최신 업데이트를 갖추도록 확인하고 CLI 구성 요소의 안정성을 보장합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="a32f9-107">수동으로 설치하기 전에 배포에 필요한 패키지가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a32f9-108">필수 조건</span><span class="sxs-lookup"><span data-stu-id="a32f9-108">Prerequisites</span></span>

<span data-ttu-id="a32f9-109">CLI에는 다음과 같은 소프트웨어가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-109">The CLI requires the following software:</span></span>

* [<span data-ttu-id="a32f9-110">Python 2.7 또는 Python 3.x</span><span class="sxs-lookup"><span data-stu-id="a32f9-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="a32f9-111">libffi</span><span class="sxs-lookup"><span data-stu-id="a32f9-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="a32f9-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="a32f9-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="a32f9-113">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="a32f9-113">Install or update</span></span>

<span data-ttu-id="a32f9-114">CLI 설치 및 업데이트 모두 설치 스크립트를 다시 실행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-114">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="a32f9-115">`curl`을 실행하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-115">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="a32f9-116">또한 스크립트를 다운로드하여 로컬로 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-116">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="a32f9-117">변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="a32f9-118">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="a32f9-119">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a32f9-120">다른 인증 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a32f9-120">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a32f9-121">문제 해결</span><span class="sxs-lookup"><span data-stu-id="a32f9-121">Troubleshooting</span></span>

<span data-ttu-id="a32f9-122">수동 설치 중에 몇 가지 공통 문제가 발견됐습니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="a32f9-123">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a32f9-123">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="a32f9-124">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="a32f9-124">curl "Object Moved" error</span></span>

<span data-ttu-id="a32f9-125">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="a32f9-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="a32f9-126">`az` 명령을 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="a32f9-126">`az` command not found</span></span>

<span data-ttu-id="a32f9-127">설치 후 명령을 실행할 수 없는 경우 `bash` 또는 `zsh`를 이용해 셸의 명령 해시 캐시를 지웁니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="a32f9-128">실행</span><span class="sxs-lookup"><span data-stu-id="a32f9-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="a32f9-129">한 다음 문제가 해결되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="a32f9-130">설치 후 셸을 다시 시작하지 않아도 이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-130">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="a32f9-131">`az` 명령의 위치가 `$PATH`여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="a32f9-132">`az` 명령의 위치는</span><span class="sxs-lookup"><span data-stu-id="a32f9-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="a32f9-133">제거</span><span class="sxs-lookup"><span data-stu-id="a32f9-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="a32f9-134">설치 시 선택한 위치에서 파일을 직접 삭제하여 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="a32f9-135">기본 설치 위치는 `$HOME`입니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="a32f9-136">설치된 CLI 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```

2. <span data-ttu-id="a32f9-137">`$HOME/.bash_profile` 파일을 수정하여 다음 선을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="a32f9-138">`bash` 또는 `zsh`를 사용하는 경우 셸의 명령 캐시를 다시 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="a32f9-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```

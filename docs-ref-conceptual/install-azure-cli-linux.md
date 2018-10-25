---
title: Linux용 Azure CLI 수동 설치
description: Linux용 Azure CLI를 수동으로 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 38d32f62cbaff7d5f1bdf7fd52bf00d47e9e14b1
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652501"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="c0447-103">Linux에 Azure CLI 수동 설치</span><span class="sxs-lookup"><span data-stu-id="c0447-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="c0447-104">배포를 위한 Azure CLI용 패키지가 없다면 스크립트를 실행하여 수동으로 CLI를 설치하십시오.</span><span class="sxs-lookup"><span data-stu-id="c0447-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

> [!NOTE]
> <span data-ttu-id="c0447-105">패키지 관리자를 사용하여 CLI를 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="c0447-106">패키지 관리자가 항상 최신 업데이트를 갖추도록 확인하고 CLI 구성 요소의 안정성을 보장합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="c0447-107">수동으로 설치하기 전에 배포에 필요한 패키지가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0447-108">필수 조건</span><span class="sxs-lookup"><span data-stu-id="c0447-108">Prerequisites</span></span>

<span data-ttu-id="c0447-109">CLI에는 다음과 같은 소프트웨어가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-109">The CLI requires the following software:</span></span>

* [<span data-ttu-id="c0447-110">Python 2.7 또는 Python 3.x</span><span class="sxs-lookup"><span data-stu-id="c0447-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="c0447-111">libffi</span><span class="sxs-lookup"><span data-stu-id="c0447-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="c0447-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="c0447-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="c0447-113">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="c0447-113">Install or update</span></span>

<span data-ttu-id="c0447-114">CLI 설치 및 업데이트 모두 설치 스크립트를 다시 실행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-114">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="c0447-115">`curl`을 실행하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-115">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="c0447-116">또한 스크립트를 다운로드하여 로컬로 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-116">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="c0447-117">변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="c0447-118">그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c0447-119">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="c0447-120">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c0447-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c0447-121">문제 해결</span><span class="sxs-lookup"><span data-stu-id="c0447-121">Troubleshooting</span></span>

<span data-ttu-id="c0447-122">수동 설치 중에 몇 가지 공통 문제가 발견됐습니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="c0447-123">여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c0447-123">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="c0447-124">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="c0447-124">curl "Object Moved" error</span></span>

<span data-ttu-id="c0447-125">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="c0447-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="c0447-126">`az` 명령을 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="c0447-126">`az` command not found</span></span>

<span data-ttu-id="c0447-127">설치 후 명령을 실행할 수 없는 경우 `bash` 또는 `zsh`를 이용해 셸의 명령 해시 캐시를 지웁니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="c0447-128">실행</span><span class="sxs-lookup"><span data-stu-id="c0447-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="c0447-129">한 다음 문제가 해결되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="c0447-130">설치 후 셸을 다시 시작하지 않아도 이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-130">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="c0447-131">`az` 명령의 위치가 `$PATH`여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="c0447-132">`az` 명령의 위치는</span><span class="sxs-lookup"><span data-stu-id="c0447-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="c0447-133">제거</span><span class="sxs-lookup"><span data-stu-id="c0447-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="c0447-134">설치 시 선택한 위치에서 파일을 직접 삭제하여 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="c0447-135">기본 설치 위치는 `$HOME`입니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="c0447-136">설치된 CLI 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-136">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="c0447-137">`$HOME/.bash_profile` 파일을 수정하여 다음 선을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="c0447-138">`bash` 또는 `zsh`를 사용하는 경우 셸의 명령 캐시를 다시 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="c0447-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="c0447-139">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c0447-139">Next Steps</span></span>

<span data-ttu-id="c0447-140">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="c0447-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c0447-141">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="c0447-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

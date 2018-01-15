---
title: "Linux용 Azure CLI 2.0 수동 설치"
description: "Linux용 Azure CLI 2.0을 수동으로 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure linux, azure 설치 linux"
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
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="0fc92-104">Linux에 Azure CLI 2.0 수동 설치</span><span class="sxs-lookup"><span data-stu-id="0fc92-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="0fc92-105">배포에 사용할 수 있는 Azure CLI용 패키지가 없는 경우 언제든지 설치 스크립트를 실행하여 수동으로 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="0fc92-106">사용 가능한 패키지가 있는 경우 언제나 권장하는 설치 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fc92-107">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="0fc92-107">Prerequisites</span></span>

<span data-ttu-id="0fc92-108">CLI를 설치하려면 시스템에 다음과 같은 소프트웨어가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="0fc92-109">Python 2.7 또는 Python 3.x</span><span class="sxs-lookup"><span data-stu-id="0fc92-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="0fc92-110">libffi</span><span class="sxs-lookup"><span data-stu-id="0fc92-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="0fc92-111">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="0fc92-111">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="0fc92-112">수동으로 설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="0fc92-112">Install or update manually</span></span>

<span data-ttu-id="0fc92-113">CLI를 설치하든 또는 업데이트하는, 전체 설치를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="0fc92-114">필수 구성 요소를 모두 갖춘 후에는 `curl`을 실행하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="0fc92-115">원하는 경우 또는 시스템에 `curl`이 없는 경우 스크립트를 다운로드하여 로컬로 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="0fc92-116">변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="0fc92-117">설치 후 `az` 명령을 사용하여 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0fc92-118">문제 해결</span><span class="sxs-lookup"><span data-stu-id="0fc92-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="0fc92-119">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="0fc92-119">curl "Object Moved" error</span></span>

<span data-ttu-id="0fc92-120">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="0fc92-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="0fc92-121">`az` 명령을 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="0fc92-121">`az` command not found</span></span>

<span data-ttu-id="0fc92-122">설치 후 명령을 실행할 수 없는 경우 셸의 명령 해시 캐시를 지워야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="0fc92-123">실행</span><span class="sxs-lookup"><span data-stu-id="0fc92-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="0fc92-124">한 다음 문제가 해결되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-124">and see if the problem is resolved.</span></span>

<span data-ttu-id="0fc92-125">설치 후 셸을 다시 시작하지 않아도 이 현상이 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="0fc92-126">`az` 명령의 위치가 `$PATH`여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="0fc92-127">설치 스크립트를 실행하면 다음과 같이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="0fc92-128">수동으로 제거</span><span class="sxs-lookup"><span data-stu-id="0fc92-128">Unstinall manually</span></span>

<span data-ttu-id="0fc92-129">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="0fc92-130">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="0fc92-131">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="0fc92-132">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="0fc92-133">설치 위치에서 파일을 직접 삭제하여 CLI를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="0fc92-134">`https://aka.ms/InstallAzureCLI` 스크립트를 통해 설치한 경우 설치 당시 설치 위치를 선택하셨을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="0fc92-135">기본 설치 위치는 `$HOME`입니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="0fc92-136">먼저 설치된 CLI 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="0fc92-137">그런 다음 `$HOME/.bash_profile` 파일을 수정하여 선을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="0fc92-138">마지막으로, 셸에서 명령 캐시를 사용하는 경우 명령 캐시를 다시 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="0fc92-139">`bash`및 `zsh` 사용자는 이 단계를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fc92-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```

---
title: Azure 클래식 CLI 설치
description: Mac, Linux 및 Windows용 Azure 클래식 CLI를 설치하여 Azure 서비스 사용 시작
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 78043f9c070626545030971dea2a8fd155ac76c2
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222466"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="e2a63-103">Azure 클래식 CLI 설치</span><span class="sxs-lookup"><span data-stu-id="e2a63-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e2a63-104">이 항목에서는 Azure 클래식 CLI를 설치하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="e2a63-105">클래식 CLI는 사용되지 않으므로 클래식 배포 모델과 함께만 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="e2a63-106">다른 모든 배포에는 [Azure CLI](/cli/azure)를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="e2a63-107">신속하게 Azure 클래식 CLI를 설치하여 Microsoft Azure에서 리소스를 만들고 관리하기 위한 오픈 소스 셸 기반 명령 집합을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="e2a63-108">컴퓨터에 크로스 플랫폼 도구를 설치하는 몇 가지 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="e2a63-109">**npm 패키지** - npm(JavaScript용 패키지 관리자)을 실행하여 Linux 배포 또는 OS에 Azure 클래식 CLI 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="e2a63-110">Node.js 및 npm이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="e2a63-111">**설치 관리자** - 설치 관리자를 다운로드하여 macOS 또는 Windows에서 손쉽게 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="e2a63-112">**Docker 컨테이너** - 즉시 실행 가능한 Docker 컨테이너에서 클래식 CLI를 사용하기 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="e2a63-113">Docker 호스트가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-113">Requires a Docker host.</span></span>

<span data-ttu-id="e2a63-114">추가 옵션 및 배경 정보는 [GitHub](https://github.com/azure/azure-xplat-cli)에서 프로젝트 리포지토리를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e2a63-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="e2a63-115">Azure 클래식 CLI가 설치되면 `azure login`에 연결하고 명령줄 인터페이스(Bash, 터미널, 명령 프롬프트 등)에서 `azure` 명령을 실행하여 Azure 리소스 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="e2a63-116">옵션 1: npm 패키지 설치</span><span class="sxs-lookup"><span data-stu-id="e2a63-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="e2a63-117">npm 패키지에서 클래식 CLI를 설치하려면 [최신 Node.js 및 npm](https://nodejs.org/en/download/package-manager/)을 다운로드하고 설치했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="e2a63-118">그런 다음 `npm install`을 실행하여 azure-cli 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="e2a63-119">Linux 배포에서는 `npm` 명령을 정상적으로 실행하기 위해 다음과 같이 `sudo`를 사용해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="e2a63-120">OS에 Node.js 및 npm을 설치하거나 업데이트해야 하는 경우 Node.js LTS 버전 4.x 이상을 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="e2a63-121">이전 버전을 사용하는 경우 설치 오류가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="e2a63-122">원한다면 [GitHub 릴리스](https://github.com/Azure/azure-xplat-cli/releases)에서 tar 파일을 다운로드할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="e2a63-123">그런 다음, 다운로드한 npm 패키지를 다음과 같이 설치합니다.(Linux 배포에서는 `sudo`를 사용해야 할 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="e2a63-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="e2a63-124">옵션 2: 설치 관리자 사용</span><span class="sxs-lookup"><span data-stu-id="e2a63-124">Option 2: Use an installer</span></span>

<span data-ttu-id="e2a63-125">Mac 또는 Windows 컴퓨터를 사용한다면, [GitHub 릴리스](https://github.com/Azure/azure-xplat-cli/releases)에서 DMG 및 MSI 설치자를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="e2a63-126">Windows에서 [웹 플랫폼 설치 관리자](https://go.microsoft.com/?linkid=9828653) 를 다운로드하여 클래식 CLI를 설치할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="e2a63-127">이 설치 관리자를 사용하면 추가적인 Azure SDK 및 명령줄 도구를 설치하는 옵션이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="e2a63-128">옵션 3: Docker 컨테이너 사용</span><span class="sxs-lookup"><span data-stu-id="e2a63-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="e2a63-129">컴퓨터를 [Docker](https://docs.docker.com/engine/understanding-docker/) 호스트로 설정한 경우 Docker 컨테이너에서 Azure 클래식 CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="e2a63-130">다음 명령을 실행합니다. Linux 배포에서는 `sudo`를 사용해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="e2a63-131">Azure 클래식 CLI 명령 실행</span><span class="sxs-lookup"><span data-stu-id="e2a63-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="e2a63-132">클래식 CLI가 설치되면 명령줄 사용자 인터페이스(Bash, 터미널, 명령 프롬프트 등)에서 `azure` 명령을 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="e2a63-133">예를 들어 help 명령을 실행하려면 다음을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-133">For example, to run the help command, type the following:</span></span>

```azurecli-interactive
azure help
```

> [!NOTE]
> <span data-ttu-id="e2a63-134">일부 Linux 배포에서 `/usr/bin/env: ‘node’: No such file or directory`과 비슷한 오류가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="e2a63-135">이 오류는 최근에 Node.js를 /usr/bin/nodejs에 설치할 때 비롯되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="e2a63-136">해결하려면 이 명령을 실행하여 /Usr/bin/node에 바로 가기 링크를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="e2a63-137">설치한 Azure 클래식 CLI의 버전을 보려면 다음을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli-interactive
azure --version
```

> [!NOTE]
> <span data-ttu-id="e2a63-138">Azure 클래식 CLI를 처음 사용할 때, 사용 정보를 Microsoft가 수집하도록 허용할 것인지 묻는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="e2a63-139">참여는 자발적입니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-139">Participation is voluntary.</span></span> <span data-ttu-id="e2a63-140">참여하기로 선택한 경우, `azure telemetry --disable`을 실행하여 언제든지 중지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="e2a63-141">언제라도 참여를 활성화하려면, `azure telemetry --enable`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="e2a63-142">클래식 CLI 업데이트</span><span class="sxs-lookup"><span data-stu-id="e2a63-142">Update the classic CLI</span></span>

<span data-ttu-id="e2a63-143">Microsoft는 업데이트된 Azure 클래식 CLI 버전을 발표할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="e2a63-144">사용 중인 운영 체제에 대 한 설치 관리자를 사용하여 클래식 CLI를 다시 설치하거나 최신 Docker 컨테이너를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="e2a63-145">또는 최신 Node.js 및 npm이 설치된 경우 다음을 입력하여 업데이트합니다.(Linux 배포에서는 `sudo`를 사용해야 할 수 있습니다)</span><span class="sxs-lookup"><span data-stu-id="e2a63-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="e2a63-146">탭 완성 기능 사용</span><span class="sxs-lookup"><span data-stu-id="e2a63-146">Enable tab completion</span></span>

<span data-ttu-id="e2a63-147">클래식 CLI 명령의 탭 완성 기능이 Mac 및 Linux에서 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="e2a63-148">zsh에서 사용하도록 설정하려면 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="e2a63-149">bash에서 사용하도록 설정하려면 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e2a63-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="e2a63-150">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e2a63-150">Next steps</span></span>

* <span data-ttu-id="e2a63-151">Azure 클래식 CLI에 대한 자세한 내용을 보거나, 소스 코드를 다운로드하거나, 문제를 보고하거나, 프로젝트에 기여하려면 [Azure 클래식 CLI에 대한 GitHub 리포지토리](https://github.com/azure/azure-xplat-cli)를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="e2a63-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>

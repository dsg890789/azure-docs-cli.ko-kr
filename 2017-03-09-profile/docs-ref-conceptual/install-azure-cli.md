---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0 설치에 대한 참조 문서입니다."
keywords: "Azure CLI, Azure CLI 설치, Azure Python CLI, Azure CLI 참조"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 5a667ad8720100b45ff714601225535ef442545c
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="769eb-104">Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="769eb-105">지금 새 버전의 Azure CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="769eb-106">Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="769eb-107">macOS, Linux 및 Windows에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="769eb-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="769eb-109">ASM(Azure 서비스 관리) 모델을 사용하는 경우 [Azure CLI 1.0을 설치합니다](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="769eb-109">If you are using the Azure Service Management (ASM) model, [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="769eb-110"><a name="macOS"/>macOS에 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="769eb-111">macOS에서는 [Homebrew](https://brew.sh/) 또는 수동으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="769eb-112">Homebrew로 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-112">Install with Homebrew</span></span>

1. <span data-ttu-id="769eb-113">아직 설치하지 않은 경우 [Homebrew 설치 지침](https://docs.brew.sh/Installation.html)에 따라 Homebrew를 설치하십시오.</span><span class="sxs-lookup"><span data-stu-id="769eb-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="769eb-114">이전에 CLI를 수동으로 설치한 경우 [수동 제거](#UninstallManually) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="769eb-115">로컬 Homebrew 리포지토리를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="769eb-116">`azure-cli` 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="769eb-117">이전에 Azure CLI 1.0을 Homebrew로 설치한 경우 패키지를 설치하는 대신 일반 Homebrew 업데이트 프로세스를 통해 CLI 2.0을 확보할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="769eb-118">수동 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-118">Install manually</span></span>

1. <span data-ttu-id="769eb-119">`curl`을 사용하여 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="769eb-120">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

3. <span data-ttu-id="769eb-121">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="769eb-122">Windows에 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="769eb-123">Windows 명령줄용 MSI를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-123">Install with MSI for the Windows command-line</span></span>

<span data-ttu-id="769eb-124">Windows에 CLI를 설치하고 Windows 명령줄에서 사용하려면 [Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다운로드하여 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="769eb-125">Windows의 Ubuntu에 있는 Bash용 apt-get을 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="769eb-126">Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="769eb-127">Bash 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="769eb-128">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="769eb-129">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="769eb-130">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-apt-package-manager"></a><span data-ttu-id="769eb-131">apt 패키지 관리자를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-131">Install with apt package manager</span></span>

<span data-ttu-id="769eb-132">Ubuntu 또는 Debian과 같은 `apt` 패키지 관리자를 사용하는 배포의 경우 `apt-get`을 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-132">For distributions using the `apt` package manager such as Ubuntu or Debian, you can install Azure CLI 2.0 via `apt-get`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="769eb-133">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-133">Modify your sources list:</span></span>

   - <span data-ttu-id="769eb-134">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="769eb-134">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="769eb-135">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="769eb-135">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="769eb-136">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-136">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="769eb-137">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-137">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-yum-package-manager"></a><span data-ttu-id="769eb-138">yum 패키지 관리자를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-138">Install with yum package manager</span></span>

<span data-ttu-id="769eb-139">Red Hat Enterprise Linux(RHEL), Fedora 또는 CentOS와 같은 `yum` 패키지 관리자를 사용하는 배포의 경우 `yum`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-139">For distributions which use the `yum` package manager such as Red Hat Enterprise Linux (RHEL), Fedora, or CentOS, you can install Azure CLI 2.0 via `yum`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="769eb-140">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-140">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="769eb-141">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-141">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="769eb-142">`yum` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-142">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="769eb-143">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-143">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-zypper-package-manager"></a><span data-ttu-id="769eb-144">zypper 패키지 관리자를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-144">Install with zypper package manager</span></span>

<span data-ttu-id="769eb-145">OpenSUSE 또는 SLE와 같은 `zypper` 패키지 관리자를 사용하는 배포의 경우 `zypper`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-145">For distributions which use the `zypper` package manager such as OpenSUSE or SLE, you can install Azure CLI 2.0 via `zypper`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="769eb-146">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-146">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="769eb-147">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-147">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="769eb-148">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-148">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="769eb-149">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-149">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="769eb-150">Docker를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-150">Install with Docker</span></span>

<span data-ttu-id="769eb-151">Azure CLI 2.0으로 미리 구성된 Docker 이미지를 유지하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-151">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="769eb-152">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-152">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="769eb-153">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-153">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="769eb-154">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-154">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="769eb-155">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-155">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="769eb-156"><a name="Linux"/>패키지 관리자를 사용하지 않고 Linux에 설치</span><span class="sxs-lookup"><span data-stu-id="769eb-156"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="769eb-157">가능한 경우 패키지 관리자를 사용하여 CLI를 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-157">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="769eb-158">Microsoft의 리포지토리를 추가하지 않거나 제공된 패키지가 없는 배포로 작업하는 경우에 CLI을 수동으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-158">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="769eb-159">Linux 배포판에 따라 필수 구성 요소를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-159">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="769eb-160">배포판이 위에 나열되지 않은 경우 [Python 2.7 이상](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) 및 [OpenSSL 1.0.2](https://www.openssl.org/source/)를 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-160">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL 1.0.2](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="769eb-161">`curl`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-161">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="769eb-162">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-162">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="769eb-163">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-163">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="769eb-164">문제 해결</span><span class="sxs-lookup"><span data-stu-id="769eb-164">Troubleshooting</span></span>

<span data-ttu-id="769eb-165">CLI 설치 중에 문제가 발생하면 이 섹션을 확인하여 해당 사례가 적용되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-165">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="769eb-166">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="769eb-166">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="769eb-167">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="769eb-167">curl "Object Moved" error</span></span>

<span data-ttu-id="769eb-168">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-168">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="769eb-169">`az` 명령을 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="769eb-169">`az` command not found</span></span>

<span data-ttu-id="769eb-170">셸의 명령 해시 캐시를 지워야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-170">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="769eb-171">실행</span><span class="sxs-lookup"><span data-stu-id="769eb-171">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="769eb-172">한 다음 문제가 해결되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-172">and see if the problem is resolved.</span></span> <span data-ttu-id="769eb-173">`$PATH`에 명령이 없을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-173">The command may also not be in your `$PATH`.</span></span> <span data-ttu-id="769eb-174">`$PATH`에 `<install path>/bin`이 표시되는지 확인하고, 필요한 경우 셸을 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-174">Make sure that `<install path>/bin` appears in your `$PATH`, and restart your shell if necessary.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="769eb-175">CLI 1.x 버전 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-175">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="769eb-176">시스템에서 이전의 CLI 1.x 버전을 사용할 수 있는 경우 사용된 설치 유형에 따라 이를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-176">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="769eb-177">npm을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-177">Uninstall with npm</span></span>

<span data-ttu-id="769eb-178">`npm uninstall`을 사용하여 이전 버전의 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-178">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="769eb-179">배포 패키지를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-179">Uninstall with distributable</span></span>

<span data-ttu-id="769eb-180">[Azure CLI 설치 관리자(MSI)](http://aka.ms/webpi-azure-cli) 또는 [macOS 패키지](http://aka.ms/mac-azure-cli)를 통해 설치한 경우 동일한 도구를 사용하여 설치를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-180">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="769eb-181">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-181">Uninstall with Docker</span></span>

<span data-ttu-id="769eb-182">Docker 이미지를 설치하여 이전 버전의 CLI를 사용한 경우 해당 이미지 및 관련 컨테이너를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-182">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="769eb-183">그런 다음 설치 지침에서 설명하는 대로 새 Docker 이미지를 설치한 후 컨테이너를 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-183">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="769eb-184">CLI 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-184">Update the CLI</span></span>

<span data-ttu-id="769eb-185">Azure CLI를 업데이트하려면 설치하는 데 사용된 동일한 방법을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-185">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="769eb-186">Homebrew로 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-186">Update with Homebrew</span></span>

1. <span data-ttu-id="769eb-187">이전에 수동으로 설치한 경우 [Homebrew로 설치](#macOS) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-187">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="769eb-188">로컬 Homebrew 리포지토리 정보를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-188">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="769eb-189">설치된 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-189">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="769eb-190">MSI를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-190">Update with MSI</span></span>

<span data-ttu-id="769eb-191">[Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-191">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt"></a><span data-ttu-id="769eb-192">apt를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-192">Update with apt</span></span>

<span data-ttu-id="769eb-193">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-193">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="769eb-194">이렇게 하면 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-194">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="769eb-195">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-195">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-yum"></a><span data-ttu-id="769eb-196">yum을 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-196">Update with yum</span></span>

<span data-ttu-id="769eb-197">`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-197">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a><span data-ttu-id="769eb-198">zypper를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-198">Update with zypper</span></span>

<span data-ttu-id="769eb-199">`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-199">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a><span data-ttu-id="769eb-200">Docker를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-200">Update with Docker</span></span>

1. <span data-ttu-id="769eb-201">`docker pull`을 사용하여 로컬 이미지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-201">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="769eb-202">현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-202">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="769eb-203">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-203">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="769eb-204">컨테이너를 중지하고 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-204">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="769eb-205">수동으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="769eb-205">Update manually</span></span>

<span data-ttu-id="769eb-206">[macOS](#macOS) 또는 [Linux](#Linux)에 대한 수동 설치 지침에 따라 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-206">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="769eb-207">제거</span><span class="sxs-lookup"><span data-stu-id="769eb-207">Uninstall</span></span>

<span data-ttu-id="769eb-208">CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-208">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="769eb-209">CLI를 설치하는 데 사용한 동일한 방법을 사용하여 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-209">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="769eb-210">Homebrew로 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-210">Uninstall with Homebrew</span></span>

<span data-ttu-id="769eb-211">`azure-cli` 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-211">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="769eb-212">MSI를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-212">Uninstall with MSI</span></span>

<span data-ttu-id="769eb-213">[MSI](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-213">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt"></a><span data-ttu-id="769eb-214">apt를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-214">Uninstall with apt</span></span>

<span data-ttu-id="769eb-215">`apt-get remove`를 통해 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-215">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a><span data-ttu-id="769eb-216">yum을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-216">Uninstall with yum</span></span>

1. <span data-ttu-id="769eb-217">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-217">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="769eb-218">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-218">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="769eb-219">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-219">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a><span data-ttu-id="769eb-220">zypper를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-220">Uninstall with zypper</span></span>

1. <span data-ttu-id="769eb-221">시스템에서 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-221">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="769eb-222">CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-222">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="769eb-223">리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-223">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="769eb-224">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-224">Uninstall with Docker</span></span>

<span data-ttu-id="769eb-225">Docker 이미지를 설치한 경우 이를 실행하는 컨테이너를 모두 제거한 다음 로컬 이미지를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-225">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="769eb-226">azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-226">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="769eb-227">CLI 이미지가 있는 컨테이너를 모두 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-227">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="769eb-228">로컬로 설치된 CLI 이미지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-228">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="769eb-229">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-229">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="769eb-230"><a name="UninstallManually"/>수동으로 제거</span><span class="sxs-lookup"><span data-stu-id="769eb-230"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="769eb-231">https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-231">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="769eb-232">설치된 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-232">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="769eb-233">`<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-233">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="769eb-234">셸에서 명령 캐시를 사용하는 경우 다시 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="769eb-234">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="769eb-235">기본 설치 위치는 macOS은 `/Users/<username>`, Linux는 `/home/<username>`입니다</span><span class="sxs-lookup"><span data-stu-id="769eb-235">The default install location is `/Users/<username>` for macOS and `/home/<username>` for Linux.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="769eb-236">CLI 문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="769eb-236">Report CLI issues and feedback</span></span>

<span data-ttu-id="769eb-237">도구에서 버그가 발생하면 GitHub 리포지토리의 [Issues](https://github.com/Azure/azure-cli/issues) 섹션에서 문제를 제출해 주세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-237">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="769eb-238">명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 주세요.</span><span class="sxs-lookup"><span data-stu-id="769eb-238">To provide feedback from the command line, use the `az feedback` command.</span></span>

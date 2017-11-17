---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0 설치에 대한 참조 문서입니다."
keywords: "Azure CLI 2.0, Azure CLI 2.0 참조, Azure CLI 2.0 설치, Azure Python CLI, Azure CLI 2.0 제거, Azure CLI, Azure CLI 설치, Azure CLI 참조"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 00d5b555975007d7e57f04ce5d69f4f29e6d0219
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="66ab9-104">Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="66ab9-105">지금 새 버전의 Azure CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="66ab9-106">Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="66ab9-107">macOS, Linux 및 Windows에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="66ab9-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="66ab9-109">이전 버전의 Azure CLI가 필요한 경우 [Azure CLI 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="66ab9-110"><a name="macOS"/>macOS에 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="66ab9-111">`curl`을 사용하여 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="66ab9-112">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="66ab9-113">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="66ab9-114">Windows에 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-114">Install on Windows</span></span>

<span data-ttu-id="66ab9-115">MSI를 사용하여 Azure CLI 2.0을 설치하고 Windows 명령줄에서 사용할 수 있거나 `apt-get`을 사용하여 Windows의 Ubuntu에 있는 Bash에 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="66ab9-116">Windows 명령줄용 MSI를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="66ab9-117">Windows에 CLI를 설치하고 Windows 명령줄에서 사용하려면 [MSI](https://aka.ms/InstallAzureCliWindows)를 다운로드하여 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="66ab9-118">Windows의 Ubuntu에 있는 Bash용 apt-get을 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="66ab9-119">Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="66ab9-120">Bash 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="66ab9-121">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="66ab9-122">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="66ab9-123">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="66ab9-124">apt-get을 사용하여 Debian/Ubuntu에 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="66ab9-125">Debian/Ubuntu 기반 시스템의 경우 `apt-get`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="66ab9-126">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-126">Modify your sources list.</span></span>
 
   - <span data-ttu-id="66ab9-127">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="66ab9-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="66ab9-128">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="66ab9-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="66ab9-129">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="66ab9-130">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="66ab9-131">Docker를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-131">Install with Docker</span></span>

<span data-ttu-id="66ab9-132">Azure CLI 2.0으로 미리 구성된 Docker 이미지를 유지하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-132">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="66ab9-133">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-133">Install the CLI using `docker run`.</span></span>

  ```bash
  docker run azuresdk/azure-cli-python:<version>
  ```

<span data-ttu-id="66ab9-134">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-134">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="66ab9-135">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-135">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="66ab9-136">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-136">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="66ab9-137"><a name="Linux"/>apt-get을 사용하지 않고 Linux에 설치</span><span class="sxs-lookup"><span data-stu-id="66ab9-137"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="66ab9-138">가능한 경우 `apt-get`을 사용하여 CLI를 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-138">It is recommended that you install the CLI with `apt-get` if you are able to.</span></span> <span data-ttu-id="66ab9-139">`apt` 패키지 관리자를 사용하지 않는 배포판의 경우 수동으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-139">For distributions which do not use the `apt` package manager, you can manually install.</span></span>

1. <span data-ttu-id="66ab9-140">Linux 배포판에 따라 필수 구성 요소를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-140">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="66ab9-141">위에서 배포판이 나열되지 않으면 [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) 및 [OpenSSL](https://www.openssl.org/source/)을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-141">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="66ab9-142">`curl`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-142">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="66ab9-143">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-143">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="66ab9-144">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-144">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="66ab9-145">문제 해결</span><span class="sxs-lookup"><span data-stu-id="66ab9-145">Troubleshooting</span></span>

<span data-ttu-id="66ab9-146">CLI 설치 중에 문제가 발생하면 이 섹션을 확인하여 해당 사례가 적용되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-146">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="66ab9-147">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="66ab9-147">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="66ab9-148">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="66ab9-148">curl "Object Moved" error</span></span>

<span data-ttu-id="66ab9-149">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-149">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="66ab9-150">이전 버전을 설치하는 macOS의 Homebrew</span><span class="sxs-lookup"><span data-stu-id="66ab9-150">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="66ab9-151">macOS에서 사용할 수 있는 `azure-cli` Homebrew 수식은 현재 유효 기간이 만료되었으며 CLI 1.x 버전을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-151">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="66ab9-152">`brew info azure-cli`를 확인하여 업데이트 시기를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-152">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="66ab9-153">이때까지 [이전 버전을 제거](#uninstall_brew)하고 [macOS 설치 지침](#macOS)을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-153">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="66ab9-154">CLI 1.x 버전 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-154">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="66ab9-155">시스템에서 이전의 CLI 1.x 버전을 사용할 수 있는 경우 사용된 설치 유형에 따라 이를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-155">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="66ab9-156">npm을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-156">Uninstall with npm</span></span>

<span data-ttu-id="66ab9-157">`npm uninstall`을 사용하여 이전 버전의 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-157">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="66ab9-158"><a name="uninstall_brew"/>macOS에서 Homebrew를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-158"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="66ab9-159">`brew uninstall`을 사용하여 이전 버전의 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-159">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="66ab9-160">배포 패키지를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-160">Uninstall with distributable</span></span>

<span data-ttu-id="66ab9-161">[MSI](http://aka.ms/webpi-azure-cli) 또는 [macOS 패키지](http://aka.ms/mac-azure-cli)를 통해 설치한 경우 동일한 도구를 사용하여 설치를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-161">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="66ab9-162">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-162">Uninstall with Docker</span></span>

<span data-ttu-id="66ab9-163">Docker 이미지를 설치하여 이전 버전의 CLI를 사용한 경우 해당 이미지 및 관련 컨테이너를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-163">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="66ab9-164">그런 다음 설치 지침에서 설명하는 대로 새 Docker 이미지를 설치한 후 컨테이너를 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-164">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="66ab9-165">CLI 업데이트</span><span class="sxs-lookup"><span data-stu-id="66ab9-165">Update the CLI</span></span>

<span data-ttu-id="66ab9-166">Azure CLI를 업데이트하려면 설치하는 데 사용된 동일한 방법을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-166">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="66ab9-167">MSI를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="66ab9-167">Update with MSI</span></span>

<span data-ttu-id="66ab9-168">[MSI](https://aka.ms/InstallAzureCliWindows)를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-168">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="66ab9-169">apt-get을 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="66ab9-169">Update with apt-get</span></span>

<span data-ttu-id="66ab9-170">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-170">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="66ab9-171">이렇게 하면 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-171">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="66ab9-172">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-172">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="66ab9-173">Docker를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="66ab9-173">Update with Docker</span></span>

1. <span data-ttu-id="66ab9-174">`docker pull`을 사용하여 로컬 이미지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-174">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="66ab9-175">현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-175">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="66ab9-176">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-176">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="66ab9-177">컨테이너를 중지하고 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-177">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="66ab9-178">수동으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="66ab9-178">Update manually</span></span>

<span data-ttu-id="66ab9-179">[macOS](#macOS) 또는 [Linux](#Linux)에 대한 수동 설치 지침에 따라 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-179">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="66ab9-180">제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-180">Uninstall</span></span>

<span data-ttu-id="66ab9-181">CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-181">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="66ab9-182">CLI를 설치하는 데 사용한 동일한 방법을 사용하여 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-182">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="66ab9-183">MSI를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-183">Uninstall with MSI</span></span>

<span data-ttu-id="66ab9-184">[MSI](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-184">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="66ab9-185">apt-get을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-185">Uninstall with apt-get</span></span>

<span data-ttu-id="66ab9-186">`apt-get remove`를 통해 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-186">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="66ab9-187">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-187">Uninstall with Docker</span></span>

<span data-ttu-id="66ab9-188">Docker 이미지를 설치한 경우 이를 실행하는 컨테이너를 모두 제거한 다음 로컬 이미지를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-188">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="66ab9-189">azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-189">Get the containers which are running the azure-cli image.</span></span>

  ```bash
  docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
  ```

  ```output
  CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
  34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
  ```

2. <span data-ttu-id="66ab9-190">CLI 이미지가 있는 컨테이너를 모두 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-190">Delete any containers with the CLI image.</span></span>

  ```bash
  docker rm 34a868beb2ab
  ```

3. <span data-ttu-id="66ab9-191">로컬로 설치된 CLI 이미지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-191">Remove the locally installed CLI image.</span></span>

  ```bash
  docker rmi azuresdk/azure-cli-python
  ```

> [!NOTE]
> <span data-ttu-id="66ab9-192">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-192">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="66ab9-193">수동으로 제거</span><span class="sxs-lookup"><span data-stu-id="66ab9-193">Uninstall manually</span></span>

<span data-ttu-id="66ab9-194">https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-194">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="66ab9-195">설치된 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-195">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="66ab9-196">`<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-196">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="66ab9-197">기본 설치 위치는 `/Users/<username>`입니다.</span><span class="sxs-lookup"><span data-stu-id="66ab9-197">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="66ab9-198">CLI 문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="66ab9-198">Report CLI issues and feedback</span></span>

<span data-ttu-id="66ab9-199">도구에서 버그가 발생하면 GitHub 리포지토리의 [Issues](https://github.com/Azure/azure-cli/issues) 섹션에서 문제를 제출해 주세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-199">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="66ab9-200">명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 주세요.</span><span class="sxs-lookup"><span data-stu-id="66ab9-200">To provide feedback from the command line, use the `az feedback` command.</span></span>

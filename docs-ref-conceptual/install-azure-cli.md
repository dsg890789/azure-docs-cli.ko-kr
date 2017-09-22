---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0 설치에 대한 참조 문서"
keywords: "Azure CLI 2.0, Azure CLI 2.0 참조, Azure CLI 2.0 설치, Azure Python CLI, Azure CLI 2.0 제거"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 08/17/2017
ms.topic: "articleå"
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 432edac070e238a6f1be0ccd76b9b3582b082219
ms.sourcegitcommit: 2ec80224c6b831e31038b710d912c0dbb1ddfef6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/17/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="80715-104">Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="80715-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="80715-105">지금 새 버전의 Azure CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="80715-106">Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="80715-107">macOS, Linux 및 Windows에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="80715-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="80715-109">이전 버전의 Azure CLI가 필요한 경우 [Azure CLI 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="80715-110">macOS</span><span class="sxs-lookup"><span data-stu-id="80715-110">macOS</span></span>

> [!WARNING]
> <span data-ttu-id="80715-111">Azure CLI의 Homebrew 수식 `azure-cli` 현재 최신이 아니며 이전 버전을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-111">The Homebrew formula for the Azure CLI, `azure-cli`, is currently out of date and will install a previous version.</span></span>

1. <span data-ttu-id="80715-112">`curl` 명령 하나로 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-112">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="80715-113">일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-113">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="80715-114">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-114">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="80715-115">InstallAzureCli로 설치할 경우 [`az component update`](/cli/azure/component#update)가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-115">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="80715-116">최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-116">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="80715-117">제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-117">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="80715-118">Windows</span><span class="sxs-lookup"><span data-stu-id="80715-118">Windows</span></span>

<span data-ttu-id="80715-119">MSI를 사용하여 Azure CLI 2.0을 설치하고 Windows 명령줄에서 사용하거나 Windows의 Ubuntu에서 Bash에 apt-get을 사용하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-119">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="80715-120">Windows 명령줄용 MSI</span><span class="sxs-lookup"><span data-stu-id="80715-120">MSI for the Windows command-line</span></span> 

<span data-ttu-id="80715-121">Windows에서 CLI를 설치하고 Windows 명령줄에서 사용하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다운로드한 후 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-121">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="80715-122">MSI를 사용하여 설치하는 경우 [`az component`](/cli/azure/component)가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-122">When you install with the msi, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="80715-123">최신 CLI로 업데이트하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-123">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="80715-124">CLI를 제거하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-124">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="80715-125">Windows의 Ubuntu에 있는 Bash의 apt-get</span><span class="sxs-lookup"><span data-stu-id="80715-125">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="80715-126">Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="80715-127">Bash 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="80715-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="80715-128">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="80715-129">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="80715-130">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-130">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="80715-131">apt-get을 사용하여 설치하는 경우 [`az component`](/cli/azure/component)가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-131">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="80715-132">CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-132">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="80715-133">제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-133">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="apt-get-for-debianubuntu"></a><span data-ttu-id="80715-134">Debian/Ubuntu 용 apt-get</span><span class="sxs-lookup"><span data-stu-id="80715-134">apt-get for Debian/Ubuntu</span></span>

<span data-ttu-id="80715-135">Debian/Ubuntu 기반 시스템의 경우 `apt-get`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-135">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="80715-136">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-136">Modify your sources list.</span></span>
 
   - <span data-ttu-id="80715-137">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="80715-137">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="80715-138">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="80715-138">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="80715-139">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-139">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="80715-140">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-140">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="80715-141">apt-get을 사용하여 설치하는 경우 [`az component`](/cli/azure/component)가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-141">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="80715-142">CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-142">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="80715-143">제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-143">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="docker"></a><span data-ttu-id="80715-144">Docker</span><span class="sxs-lookup"><span data-stu-id="80715-144">Docker</span></span>

<span data-ttu-id="80715-145">Azure CLI 2.0으로 미리 구성된 Docker 이미지를 유지하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-145">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="80715-146">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-146">Install the CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="80715-147">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-147">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="80715-148">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-148">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

>> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

<span data-ttu-id="80715-149">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="80715-149">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="80715-150">Docker 이미지는 [`az component`](/cli/azure/component) 기능을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-150">The Docker image does not support the [`az component`](/cli/azure/component) feature.</span></span>
> <span data-ttu-id="80715-151">Azure CLI 2.0을 업데이트하려면 `docker run`을 사용하여 최신 이미지 또는 원하는 특정 이미지를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-151">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="linux"></a><span data-ttu-id="80715-152">Linux</span><span class="sxs-lookup"><span data-stu-id="80715-152">Linux</span></span>

1. <span data-ttu-id="80715-153">[Python](https://www.python.org/downloads)이 없을 경우 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-153">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="80715-154">Linux 배포에 따라 필수 구성 요소를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-154">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

3. <span data-ttu-id="80715-155">하나의 `curl` 명령으로 CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-155">Install the CLI with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

4. <span data-ttu-id="80715-156">일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-156">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

5. <span data-ttu-id="80715-157">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-157">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="80715-158">InstallAzureCli로 설치할 경우 [`az component update`](/cli/azure/component#update)가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-158">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="80715-159">최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-159">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="80715-160">제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-160">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="80715-161">문제 해결</span><span class="sxs-lookup"><span data-stu-id="80715-161">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="80715-162">curl 리디렉션 관련 오류</span><span class="sxs-lookup"><span data-stu-id="80715-162">Errors with curl redirection</span></span>

<span data-ttu-id="80715-163">`curl` 명령에서 `-L` 매개 변수와 관련한 오류나 "개체 이동됨"이라는 오류가 발생할 경우 aka.ms url 대신 전체 url을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="80715-163">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="80715-164">제거</span><span class="sxs-lookup"><span data-stu-id="80715-164">Uninstall</span></span>

<span data-ttu-id="80715-165">https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80715-165">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="80715-166">설치된 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-166">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="80715-167">`<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="80715-167">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="80715-168">기본 설치 위치는 `/Users/<username>`입니다.</span><span class="sxs-lookup"><span data-stu-id="80715-168">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="80715-169">apt-get, Docker 또는 msi를 사용하여 CLI를 설치한 경우 동일한 도구를 사용하여 제거하세요.</span><span class="sxs-lookup"><span data-stu-id="80715-169">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="80715-170">문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="80715-170">Reporting issues and feedback</span></span>

<span data-ttu-id="80715-171">도구에서 버그가 발견되면 GitHub 리포지토리의 [문제](https://github.com/Azure/azure-cli/issues) 섹션에 문제를 기록해 주세요.</span><span class="sxs-lookup"><span data-stu-id="80715-171">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="80715-172">명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="80715-172">To provide feedback from the command line, try the `az feedback` command.</span></span>

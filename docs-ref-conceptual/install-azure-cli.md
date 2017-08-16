---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0에 대한 참조 문서"
keywords: "Azure CLI 2.0, Azure CLI 2.0 참조, Azure CLI 2.0 설치, Azure Python CLI, Azure CLI 2.0 제거"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.contentlocale: ko-KR
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="6f19f-104">Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="6f19f-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="6f19f-105">지금 새 버전의 Azure CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="6f19f-106">Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="6f19f-107">macOS, Linux 및 Windows에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="6f19f-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="6f19f-109">이전 버전의 Azure CLI가 필요할 경우 [Azure 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-109">If you need the previous version of the Azure CLI, here's how to [install Azure 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="6f19f-110">macOS</span><span class="sxs-lookup"><span data-stu-id="6f19f-110">macOS</span></span>

1. <span data-ttu-id="6f19f-111">`curl` 명령 하나로 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-111">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="6f19f-112">일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-112">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="6f19f-113">명령 프롬프트에서 `az` 명령을 사용하여 Azure CLI 2.0을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-113">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="6f19f-114">InstallAzureCli를 함께 설치할 경우 `az component update`가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-114">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="6f19f-115">최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-115">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="6f19f-116">제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-116">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="6f19f-117">Windows</span><span class="sxs-lookup"><span data-stu-id="6f19f-117">Windows</span></span>

<span data-ttu-id="6f19f-118">MSI를 사용하여 CLI를 설치하고 Windows 명령줄에서 사용하거나 Windows의 Ubuntu에 있는 Bash에서 apt-get을 사용하여 CLI를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-118">You can install the CLI with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="6f19f-119">Windows 명령줄용 MSI</span><span class="sxs-lookup"><span data-stu-id="6f19f-119">MSI for the Windows command-line</span></span> 

<span data-ttu-id="6f19f-120">Windows에서 CLI를 설치하고 Windows 명령줄에서 사용하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다운로드한 후 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-120">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="6f19f-121">MSI를 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-121">When you install with the msi, `az component` isn't supported.</span></span>
> <span data-ttu-id="6f19f-122">최신 CLI로 업데이트하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-122">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="6f19f-123">CLI를 제거하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-123">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="6f19f-124">Windows의 Ubuntu에 있는 Bash의 apt-get</span><span class="sxs-lookup"><span data-stu-id="6f19f-124">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="6f19f-125">Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-125">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="6f19f-126">Bash 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-126">Open the Bash shell.</span></span>

3. <span data-ttu-id="6f19f-127">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-127">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="6f19f-128">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-128">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="6f19f-129">apt-get을 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-129">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="6f19f-130">CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-130">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="6f19f-131">제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-131">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux"></a><span data-ttu-id="6f19f-132">Linux</span><span class="sxs-lookup"><span data-stu-id="6f19f-132">Linux</span></span>

1. <span data-ttu-id="6f19f-133">Linux에서는 특정 [필수 구성 요소](#linux-prerequisites)를 설치해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-133">On Linux, you may need to install specific [prerequisites](#linux-prerequisites).</span></span>

2. <span data-ttu-id="6f19f-134">`curl` 명령 하나로 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-134">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="6f19f-135">일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-135">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="6f19f-136">명령 프롬프트에서 `az` 명령을 사용하여 Azure CLI 2.0을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-136">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="6f19f-137">InstallAzureCli를 함께 설치할 경우 `az component update`가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-137">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="6f19f-138">최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-138">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="6f19f-139">제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-139">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="docker"></a><span data-ttu-id="6f19f-140">Docker</span><span class="sxs-lookup"><span data-stu-id="6f19f-140">Docker</span></span>

<span data-ttu-id="6f19f-141">Microsoft는 Azure CLI로 미리 구성된 Docker 이미지를 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-141">We maintain a Docker image preconfigured with the Azure CLI.</span></span>

<span data-ttu-id="6f19f-142">`docker run`을 사용하여 Azure CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-142">Install the Azure CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="6f19f-143">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-143">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="6f19f-144">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-144">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> <span data-ttu-id="6f19f-145">Docker 이미지는 [`component` 기능](/cli/azure/component)을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-145">The Docker image does not support the [`component` feature](/cli/azure/component).</span></span>
> <span data-ttu-id="6f19f-146">Azure CLI 2.0을 업데이트하려면 `docker run`을 사용하여 최신 이미지 또는 원하는 특정 이미지를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-146">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="apt-get"></a><span data-ttu-id="6f19f-147">apt-get</span><span class="sxs-lookup"><span data-stu-id="6f19f-147">apt-get</span></span>

<span data-ttu-id="6f19f-148">Debian/Ubuntu 기반 시스템의 경우 `apt-get`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-148">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="6f19f-149">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-149">Modify your sources list.</span></span>

   - <span data-ttu-id="6f19f-150">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="6f19f-150">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="6f19f-151">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="6f19f-151">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="6f19f-152">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-152">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="6f19f-153">apt-get을 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-153">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="6f19f-154">CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-154">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="6f19f-155">제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-155">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux-prerequisites"></a><span data-ttu-id="6f19f-156">Linux 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="6f19f-156">Linux Prerequisites</span></span>

1. <span data-ttu-id="6f19f-157">[Python](https://www.python.org/downloads)이 없을 경우 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-157">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="6f19f-158">Linux 배포에 따라 필수 구성 요소를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-158">Depending on your Linux distribution, install the prerequisites.</span></span>

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

## <a name="troubleshooting"></a><span data-ttu-id="6f19f-159">문제 해결</span><span class="sxs-lookup"><span data-stu-id="6f19f-159">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="6f19f-160">curl 리디렉션 관련 오류</span><span class="sxs-lookup"><span data-stu-id="6f19f-160">Errors with curl redirection</span></span>

<span data-ttu-id="6f19f-161">`curl` 명령에서 `-L` 매개 변수와 관련한 오류나 "개체 이동됨"이라는 오류가 발생할 경우 aka.ms url 대신 전체 url을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-161">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

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

## <a name="uninstall"></a><span data-ttu-id="6f19f-162">제거</span><span class="sxs-lookup"><span data-stu-id="6f19f-162">Uninstall</span></span>

<span data-ttu-id="6f19f-163">https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-163">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="6f19f-164">설치된 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-164">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="6f19f-165">`<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-165">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="6f19f-166">기본 설치 위치는 `/Users/<username>`입니다.</span><span class="sxs-lookup"><span data-stu-id="6f19f-166">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="6f19f-167">apt-get, Docker 또는 msi를 사용하여 CLI를 설치한 경우 동일한 도구를 사용하여 제거하세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-167">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="6f19f-168">문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="6f19f-168">Reporting issues and feedback</span></span>

<span data-ttu-id="6f19f-169">도구에서 버그가 발견되면 GitHub 리포지토리의 [문제](https://github.com/Azure/azure-cli/issues) 섹션에 문제를 기록해 주세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-169">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="6f19f-170">명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="6f19f-170">To provide feedback from the command line, try the `az feedback` command.</span></span>

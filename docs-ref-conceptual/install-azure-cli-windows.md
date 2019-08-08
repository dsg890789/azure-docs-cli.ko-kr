---
title: Windows용 Azure CLI 설치
description: Windows에 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6c972ba69344f9e8bcd14a96a90e9dadb6cd8132
ms.sourcegitcommit: 61965f5d95d0dae3752ad6a0e5a93db27a623c28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68830965"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="4928e-103">Windows에 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="4928e-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="4928e-104">MSI를 통해 Azure CLI를 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="4928e-105">WSL(Linux용 Windows 하위 시스템)을 설치하는 경우 Linux 배포에 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="4928e-106">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="4928e-107">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="4928e-107">Install or update</span></span>

<span data-ttu-id="4928e-108">MSI 배포 파일은 Windows에서 Azure CLI를 설치하거나 업데이트하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="4928e-109">MSI 설치 프로그램을 사용하기 전에 현재 버전을 제거 할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4928e-110">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="4928e-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="4928e-111">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="4928e-112">PowerShell을 사용하여 Azure CLI를 설치할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="4928e-113">관리자 권한으로 PowerShell을 시작하고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'
   ```
<span data-ttu-id="4928e-114">최신 버전의 Windows용 Azure CLI를 다운로드하여 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="4928e-115">버전이 이미 설치되어 있으면 기존 버전이 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="4928e-116">설치가 완료되면 PowerShell을 다시 열어서 Azure CLI를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="4928e-117">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="4928e-118">PowerShell은 Windows 명령 프롬프트에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="4928e-119">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="4928e-120">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4928e-121">문제 해결</span><span class="sxs-lookup"><span data-stu-id="4928e-121">Troubleshooting</span></span>

<span data-ttu-id="4928e-122">Windows에 설치할 때 나타나는 몇 가지 일반적인 문제는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="4928e-123">여기서 다루지 않은 문제가 발생하면 [GitHub에서 문제를 제출](https://github.com/Azure/azure-cli/issues)하세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="4928e-124">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="4928e-124">Proxy blocks connection</span></span>

<span data-ttu-id="4928e-125">프록시에서 연결을 차단하여 MSI 설치 관리자를 다운로드할 수 없는 경우 프록시를 올바르게 구성했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="4928e-126">Windows 10의 경우 이러한 설정은 `Settings > Network & Internet > Proxy` 창에서 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="4928e-127">필요한 설정 또는 머신에서 구성을 관리할 수 있거나 고급 설정이 필요한 경우에 대해 시스템 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4928e-128">이러한 설정은 PowerShell 또는 명령 프롬프트에서 모두 CLI를 사용하여 Azure 서비스에 액세스하는 데에도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="4928e-129">이 작업은 PowerShell에서 다음 명령을 사용하여 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="4928e-130">MSI를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="4928e-131">제거</span><span class="sxs-lookup"><span data-stu-id="4928e-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="4928e-132">Windows의 "앱 및 기능" 목록에서 Azure CLI를 제거 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="4928e-133">제거 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-133">To uninstall:</span></span>

| <span data-ttu-id="4928e-134">플랫폼</span><span class="sxs-lookup"><span data-stu-id="4928e-134">Platform</span></span> | <span data-ttu-id="4928e-135">지침</span><span class="sxs-lookup"><span data-stu-id="4928e-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="4928e-136">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="4928e-136">Windows 10</span></span> | <span data-ttu-id="4928e-137">시작 > 설정 > 앱</span><span class="sxs-lookup"><span data-stu-id="4928e-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="4928e-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="4928e-138">Windows 8</span></span><br/><span data-ttu-id="4928e-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="4928e-139">Windows 7</span></span> | <span data-ttu-id="4928e-140">시작>제어판 > 프로그램 > 프로그램 제거</span><span class="sxs-lookup"><span data-stu-id="4928e-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="4928e-141">이 화면에서 __Azure CLI__ 를 프로그램 검색 창에 입력하세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="4928e-142">제거할 프로그램은 __Azure용 Microsoft CLI 2.0__ 으로 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="4928e-143">이 애플리케이션을 선택한 다음 `Uninstall` 단추를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4928e-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4928e-144">다음 단계</span><span class="sxs-lookup"><span data-stu-id="4928e-144">Next Steps</span></span>

<span data-ttu-id="4928e-145">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="4928e-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4928e-146">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="4928e-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

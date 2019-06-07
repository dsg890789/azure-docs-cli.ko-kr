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
ms.openlocfilehash: 40810b25bf776025c82b48ba7aa424369483ceeb
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516266"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="80046-103">Windows에 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="80046-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="80046-104">MSI를 통해 Azure CLI를 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="80046-105">WSL(Linux용 Windows 하위 시스템)을 설치하는 경우 Linux 배포에 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80046-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="80046-106">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80046-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="80046-107">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="80046-107">Install or update</span></span>

<span data-ttu-id="80046-108">MSI 배포 파일은 Windows에서 Azure CLI를 설치하거나 업데이트하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="80046-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="80046-109">MSI 설치 프로그램을 사용하기 전에 현재 버전을 제거 할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="80046-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="80046-110">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="80046-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="80046-111">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="80046-112">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80046-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="80046-113">PowerShell은 Windows 명령 프롬프트에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="80046-114">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="80046-115">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="80046-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="80046-116">문제 해결</span><span class="sxs-lookup"><span data-stu-id="80046-116">Troubleshooting</span></span>

<span data-ttu-id="80046-117">Windows에 설치할 때 나타나는 몇 가지 일반적인 문제는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="80046-117">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="80046-118">여기서 다루지 않은 문제가 발생하면 [GitHub에서 문제를 제출](https://github.com/Azure/azure-cli/issues)하세요.</span><span class="sxs-lookup"><span data-stu-id="80046-118">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="80046-119">프록시 연결 차단</span><span class="sxs-lookup"><span data-stu-id="80046-119">Proxy blocks connection</span></span>

<span data-ttu-id="80046-120">프록시에서 연결을 차단하여 MSI 설치 관리자를 다운로드할 수 없는 경우 프록시를 올바르게 구성했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-120">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="80046-121">Windows 10의 경우 이러한 설정은 `Settings > Network & Internet > Proxy` 창에서 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="80046-121">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="80046-122">필요한 설정 또는 머신에서 구성을 관리할 수 있거나 고급 설정이 필요한 경우에 대해 시스템 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="80046-122">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="80046-123">이러한 설정은 PowerShell 또는 명령 프롬프트에서 모두 CLI를 사용하여 Azure 서비스에 액세스하는 데에도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-123">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="80046-124">이 작업은 PowerShell에서 다음 명령을 사용하여 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-124">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="80046-125">MSI를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-125">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="80046-126">제거</span><span class="sxs-lookup"><span data-stu-id="80046-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="80046-127">Windows의 "앱 및 기능" 목록에서 Azure CLI를 제거 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="80046-127">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="80046-128">제거하려면:</span><span class="sxs-lookup"><span data-stu-id="80046-128">To uninstall:</span></span>

| <span data-ttu-id="80046-129">플랫폼</span><span class="sxs-lookup"><span data-stu-id="80046-129">Platform</span></span> | <span data-ttu-id="80046-130">지침</span><span class="sxs-lookup"><span data-stu-id="80046-130">Instructions</span></span> |
|---|---|
| <span data-ttu-id="80046-131">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="80046-131">Windows 10</span></span> | <span data-ttu-id="80046-132">시작 > 설정 > 앱</span><span class="sxs-lookup"><span data-stu-id="80046-132">Start > Settings > Apps</span></span> |
| <span data-ttu-id="80046-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="80046-133">Windows 8</span></span><br/><span data-ttu-id="80046-134">Windows 7</span><span class="sxs-lookup"><span data-stu-id="80046-134">Windows 7</span></span> | <span data-ttu-id="80046-135">시작>제어판 > 프로그램 > 프로그램 제거</span><span class="sxs-lookup"><span data-stu-id="80046-135">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="80046-136">이 화면에서 __Azure CLI__를 프로그램 검색 창에 입력하세요.</span><span class="sxs-lookup"><span data-stu-id="80046-136">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="80046-137">제거할 프로그램은 __Azure용 Microsoft CLI 2.0__으로 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="80046-137">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="80046-138">이 애플리케이션을 선택한 다음 `Uninstall` 단추를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="80046-138">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="80046-139">다음 단계</span><span class="sxs-lookup"><span data-stu-id="80046-139">Next Steps</span></span>

<span data-ttu-id="80046-140">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="80046-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="80046-141">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="80046-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

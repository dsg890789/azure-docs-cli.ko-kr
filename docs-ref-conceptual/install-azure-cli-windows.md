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
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240555"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="f20b9-103">Windows에 Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="f20b9-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="f20b9-104">MSI를 통해 Azure CLI를 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="f20b9-105">WSL(Linux용 Windows 하위 시스템)을 설치하는 경우 Linux 배포에 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="f20b9-106">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f20b9-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="f20b9-107">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="f20b9-107">Install or update</span></span>

<span data-ttu-id="f20b9-108">MSI 배포 파일은 Windows에서 Azure CLI를 설치하거나 업데이트하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="f20b9-109">MSI 설치 프로그램을 사용하기 전에 현재 버전을 제거 할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f20b9-110">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="f20b9-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="f20b9-111">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="f20b9-112">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="f20b9-113">PowerShell은 Windows 명령 프롬프트에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="f20b9-114">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f20b9-115">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f20b9-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="f20b9-116">제거</span><span class="sxs-lookup"><span data-stu-id="f20b9-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f20b9-117">Windows의 "앱 및 기능" 목록에서 Azure CLI를 제거 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="f20b9-118">제거하려면:</span><span class="sxs-lookup"><span data-stu-id="f20b9-118">To uninstall:</span></span>

| <span data-ttu-id="f20b9-119">플랫폼</span><span class="sxs-lookup"><span data-stu-id="f20b9-119">Platform</span></span> | <span data-ttu-id="f20b9-120">지침</span><span class="sxs-lookup"><span data-stu-id="f20b9-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="f20b9-121">윈도우 10</span><span class="sxs-lookup"><span data-stu-id="f20b9-121">Windows 10</span></span> | <span data-ttu-id="f20b9-122">시작 > 설정 > 앱</span><span class="sxs-lookup"><span data-stu-id="f20b9-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="f20b9-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="f20b9-123">Windows 8</span></span><br/><span data-ttu-id="f20b9-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="f20b9-124">Windows 7</span></span> | <span data-ttu-id="f20b9-125">시작>제어판 > 프로그램 > 프로그램 제거</span><span class="sxs-lookup"><span data-stu-id="f20b9-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="f20b9-126">이 화면에서 __Azure CLI__를 프로그램 검색 창에 입력하세요.</span><span class="sxs-lookup"><span data-stu-id="f20b9-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="f20b9-127">제거할 프로그램은 __Azure용 Microsoft CLI 2.0__으로 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="f20b9-128">이 애플리케이션을 선택한 다음 `Uninstall` 단추를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="f20b9-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f20b9-129">다음 단계</span><span class="sxs-lookup"><span data-stu-id="f20b9-129">Next Steps</span></span>

<span data-ttu-id="f20b9-130">Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="f20b9-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f20b9-131">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="f20b9-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

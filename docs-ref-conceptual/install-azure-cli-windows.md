---
title: Windows용 Azure CLI 설치
description: Windows에 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d662333f828c65fa709fa622de7de3a18bea58d8
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439837"
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="29933-103">Windows에 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="29933-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="29933-104">MSI를 통해 Azure CLI 이진을 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="29933-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="29933-105">WSL(Linux용 Windows 하위 시스템)을 실행하는 경우 Linux 배포에 패키지를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29933-105">If you are running the Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="29933-106">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="29933-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="29933-107">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="29933-107">Install or update</span></span>

<span data-ttu-id="29933-108">MSI 배포판은 Windows에서 `az` 명령을 설치, 업데이트 및 제거하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="29933-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="29933-109">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="29933-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="29933-110">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="29933-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="29933-111">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29933-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="29933-112">PowerShell은 Windows 명령 프롬프트에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="29933-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="29933-113">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="29933-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="29933-114">다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="29933-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="29933-115">제거</span><span class="sxs-lookup"><span data-stu-id="29933-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="29933-116">MSI를 다시 실행 하 고 "제거" 옵션을 선택하여 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29933-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="29933-117">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="29933-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

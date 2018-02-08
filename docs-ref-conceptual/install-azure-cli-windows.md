---
title: "Windows용 Azure CLI 설치"
description: "Windows에 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure 설치 windows, azure cli windows, azure windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fc84b80e44a994495ef97cf9d7ec4e4a79a5c5b3
ms.sourcegitcommit: b41c5ed4a26c771a1a32b4560131f7a65b80fd33
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/03/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="5922a-104">Windows에 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="5922a-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="5922a-105">MSI를 통해 Azure CLI 이진을 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-105">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="5922a-106">WSL(Linux용 Windows 하위 시스템)을 실행하는 경우 Linux 배포에 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-106">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="5922a-107">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="5922a-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="5922a-108">설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="5922a-108">Install or update</span></span>

<span data-ttu-id="5922a-109">MSI 배포판은 Windows에서 `az` 명령을 설치, 업데이트 및 제거하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5922a-110">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="5922a-110">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

<span data-ttu-id="5922a-111">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="5922a-112">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="5922a-113">PowerShell은 CMD에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-113">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="5922a-114">제거</span><span class="sxs-lookup"><span data-stu-id="5922a-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="5922a-115">MSI를 다시 실행 하 고 "제거" 옵션을 선택하여 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5922a-115">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> 

> [!div class="nextstepaction"]
> [<span data-ttu-id="5922a-116">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="5922a-116">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

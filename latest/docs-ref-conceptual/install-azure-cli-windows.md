---
title: "Windows용 Azure CLI 설치"
description: "Windows에 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure 설치 windows, azure cli windows, azure windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="bbeb6-104">Windows에 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="bbeb6-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="bbeb6-105">Windows에서, Windows 명령 프롬프트 또는 PowerShell을 통해 사용할 수 있는 MSI로 네이티브 이진 파일을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="bbeb6-106">WSL(Linux용 Windows 하위 시스템)을 실행하는 경우 실행 중인 배포에 사용할 수 있는 패키지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="bbeb6-107">지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="bbeb6-108">MSI를 사용하여 설치 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="bbeb6-108">Install or update with MSI</span></span>

<span data-ttu-id="bbeb6-109">MSI 배포판은 Windows에서 `az` 명령을 설치, 업데이트 및 제거하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="bbeb6-110">[MSI 설치 관리자를 다운로드](https://aka.ms/InstallAzureCliWindows)한 후 실행하여 설치 또는 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="bbeb6-111">설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="bbeb6-112">이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="bbeb6-113">MSI를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="bbeb6-113">Uninstall with MSI</span></span>

<span data-ttu-id="bbeb6-114">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="bbeb6-115">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="bbeb6-116">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="bbeb6-117">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="bbeb6-118">MSI를 다시 실행 하 고 "제거" 옵션을 선택하여 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="bbeb6-119">MSI 설치 관리자가 없는 경우 [MSI 설치 관리자를 다운로드](https://aka.ms/InstallAzureCliWindows)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbeb6-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>

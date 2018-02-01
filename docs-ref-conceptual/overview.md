---
title: Azure CLI 2.0
description: "Azure CLI 2.0의 개요입니다."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 92079f3fa17f69a560e937101aa9e6f09c3080eb
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/26/2018
---
# <a name="azure-cli-20"></a><span data-ttu-id="15543-104">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="15543-104">Azure CLI 2.0</span></span>

<span data-ttu-id="15543-105">Azure CLI 2.0은 Azure 리소스를 관리하기 위한 Azure의 새로운 명령줄 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="15543-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="15543-106">[Azure Cloud Shell](/azure/cloud-shell/overview)을 실행하는 브라우저에서 사용하거나 macOS, Linux 및 Windows에서 [설치](install-azure-cli.md)하고 명령줄에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15543-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="15543-107">Azure CLI 2.0은 명령줄에서 Azure 리소스를 관리하는 작업 및 Azure Resource Manager에 대해 작동하는 자동화 스크립트 작성 작업에 최적화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15543-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="15543-108">Azure CLI 2.0을 사용하면 간단하게 다음 명령을 입력하여 Azure 내에서 VM을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15543-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="15543-109">[Cloud Shell](/azure/cloud-shell/overview)을 사용하여 CLI 브라우저에서 실행하거나 macOS, Linux 또는 Windows에서 [설치](install-azure-cli.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="15543-109">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="15543-110">[시작](get-started-with-azure-cli.md) 문서를 읽고 CLI 사용을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="15543-110">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="15543-111">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="15543-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="15543-112">다음 샘플을 통해 Azure CLI 2.0으로 일반 시나리오를 수행하는 방법을 배울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15543-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="15543-113">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="15543-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="15543-114">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="15543-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="15543-115">Web Apps</span><span class="sxs-lookup"><span data-stu-id="15543-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="15543-116">SQL Database</span><span class="sxs-lookup"><span data-stu-id="15543-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="15543-117">각 Azure CLI 2.0 명령을 사용하는 방법이 설명된 자세한 [참고 자료](/cli/azure/)도 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="15543-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="15543-118">지금 Azure CLI 2.0을 [시작](get-started-with-azure-cli.md)하세요.</span><span class="sxs-lookup"><span data-stu-id="15543-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="15543-119">이전 버전의 CLI(Azure CLI)를 사용하는 경우 계속 사용해도 됩니다.</span><span class="sxs-lookup"><span data-stu-id="15543-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="15543-120">두 CLI를 모두 사용하는 경우 `azure`는 기존 CLI(Azure CLI)이고 `az`는 새 CLI(Azure CLI 2.0)라는 사실을 기억하세요.</span><span class="sxs-lookup"><span data-stu-id="15543-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
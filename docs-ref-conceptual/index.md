---
title: Azure CLI 2.0 개요
description: Azure CLI 2.0의 개요입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388391"
---
# <a name="azure-cli-20"></a><span data-ttu-id="0941c-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="0941c-103">Azure CLI 2.0</span></span>

<span data-ttu-id="0941c-104">Azure CLI 2.0는 Azure 리소스를 관리하기 위한 Microsoft의 플랫폼 간 명령줄 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="0941c-105">[Azure Cloud Shell](/azure/cloud-shell/overview)을 실행하는 브라우저에서 사용하거나 macOS, Linux 또는 Windows에서 [설치](install-azure-cli.md)하고 명령줄에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="0941c-106">Azure CLI 2.0은 사용하기 쉽고, Azure Resource Manager에 작동하는 자동화 스크립트 작성에 가장 적합합니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="0941c-107">Azure CLI 2.0을 사용하면 간단하게 다음 명령을 입력하여 Azure 내에서 VM을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="0941c-108">실행 또는 설치</span><span class="sxs-lookup"><span data-stu-id="0941c-108">Run or Install</span></span>

<span data-ttu-id="0941c-109">CLI를 로컬로 설치하거나 Azure Cloud Shell을 사용하여 브라우저에서 실행하거나 Docker 컨테이너에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="0941c-110">Azure Cloud Shell을 사용하여 브라우저에서 실행하려면 [Azure Cloud Shell에서 Bash 빠른 시작](/azure/cloud-shell/quickstart) 또는 [Azure Cloud Shell에서 PowerShell 빠른 시작](/azure/cloud-shell/quickstart-powershell)을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="0941c-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="0941c-111">CLI를 설치하는 방법은 [Azure CLI 2.0 설치](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0941c-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="0941c-112">Docker 컨테이너로 실행하려면 [Docker 컨테이너에서 Azure CLI 2.0 실행](run-azure-cli-docker.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="0941c-113">시작하기</span><span class="sxs-lookup"><span data-stu-id="0941c-113">Get started</span></span>

<span data-ttu-id="0941c-114">CLI 기초를 배우려면 [시작](get-started-with-azure-cli.md) 문서를 읽어보세요.</span><span class="sxs-lookup"><span data-stu-id="0941c-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="0941c-115">다음 예제에서는 몇 가지 일반적인 사용 사례를 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="0941c-116">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="0941c-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0941c-117">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="0941c-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0941c-118">Web Apps</span><span class="sxs-lookup"><span data-stu-id="0941c-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0941c-119">SQL Database</span><span class="sxs-lookup"><span data-stu-id="0941c-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="0941c-120">각 Azure CLI 2.0 명령을 사용하는 방법이 설명된 자세한 [참고 자료](/cli/azure/reference-index)도 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="0941c-121">이전 버전의 CLI(Azure CLI 1.0)를 사용하는 경우 계속 사용해도 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="0941c-122">그러나 최상의 환경을 위해 Azure CLI 2.0의 최신 버전을 사용하도록 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="0941c-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="0941c-123">두 CLI를 모두 사용하는 경우 `azure`는 기존 CLI(Azure CLI)이고 `az`는 새 CLI(Azure CLI 2.0)라는 사실을 기억하세요.</span><span class="sxs-lookup"><span data-stu-id="0941c-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>

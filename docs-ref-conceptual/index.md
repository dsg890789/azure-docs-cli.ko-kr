---
title: Azure CLI의 개요입니다.
description: Azure CLI(명령줄 인터페이스) 개요입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
---

# <a name="azure-command-line-interface-cli"></a><span data-ttu-id="bccfc-103">Azure CLI(명령줄 인터페이스)</span><span class="sxs-lookup"><span data-stu-id="bccfc-103">Azure Command-Line Interface (CLI)</span></span>

<span data-ttu-id="bccfc-104">Azure CLI(명령줄 인터페이스)는 Azure 리소스를 관리하기 위한 Microsoft의 플랫폼 간 명령줄 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-104">The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="bccfc-105">[Azure Cloud Shell](/azure/cloud-shell/overview)을 실행하는 브라우저에서 사용하거나 macOS, Linux 또는 Windows에서 [설치](install-azure-cli.md)하고 명령줄에서 실행하십시오.</span><span class="sxs-lookup"><span data-stu-id="bccfc-105">Use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="bccfc-106">Azure CLI(명령줄 인터페이스)는 사용하기 쉽고, Azure Resource Manager에 작동하는 자동화 스크립트 작성에 가장 적합합니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-106">The Azure CLI is easy to get started with, and best used for building automation scripts that work with the Azure Resource Manager.</span></span>
<span data-ttu-id="bccfc-107">Azure CLI를 사용하면 간단하게 다음 명령을 입력하여 Azure 내에서 VM을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="bccfc-108">스크립트 및 Microsoft 설명서 사이트에 작성된 Azure CLI 예제는 `bash` 셸용입니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="bccfc-109">한 줄 예제는 모든 플랫폼에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="bccfc-110">연속하는 줄을 포함하는 더 긴 예제 (`\`) 또는 변수 할당은 PowerShell을 포함하여 다른 셸에서 작동하도록 수정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-110">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="bccfc-111">실행 또는 설치</span><span class="sxs-lookup"><span data-stu-id="bccfc-111">Run or Install</span></span>

<span data-ttu-id="bccfc-112">CLI를 로컬로 설치하거나 Azure Cloud Shell을 사용하여 브라우저에서 실행하거나 Docker 컨테이너에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span> <span data-ttu-id="bccfc-113">CLI의 현재 버전을 가져오려면 `az --version`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-113">To get the current version of the CLI, run `az --version`.</span></span>

* <span data-ttu-id="bccfc-114">Azure Cloud Shell을 사용하여 브라우저에서 실행하려면 [Azure Cloud Shell에서 Bash 빠른 시작](/azure/cloud-shell/quickstart) 또는 [Azure Cloud Shell에서 PowerShell 빠른 시작](/azure/cloud-shell/quickstart-powershell)을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="bccfc-114">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="bccfc-115">CLI를 설치하는 방법은 [Azure CLI 설치](install-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bccfc-115">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="bccfc-116">Docker 컨테이너로 실행하려면 [Docker 컨테이너에서 Azure CLI 실행](run-azure-cli-docker.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-116">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="bccfc-117">Microsoft Learn을 통해 기술 쌓기</span><span class="sxs-lookup"><span data-stu-id="bccfc-117">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="bccfc-118">Azure CLI로 가상 머신 만들기</span><span class="sxs-lookup"><span data-stu-id="bccfc-118">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="bccfc-119">CLI를 사용하여 Azure 서비스 제어</span><span class="sxs-lookup"><span data-stu-id="bccfc-119">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="bccfc-120">더 많은 대화형 학습 보기...</span><span class="sxs-lookup"><span data-stu-id="bccfc-120">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="bccfc-121">시작하기</span><span class="sxs-lookup"><span data-stu-id="bccfc-121">Get started</span></span>

<span data-ttu-id="bccfc-122">CLI 기초를 배우려면 [시작](get-started-with-azure-cli.md) 문서를 읽어보세요.</span><span class="sxs-lookup"><span data-stu-id="bccfc-122">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="bccfc-123">다음 예제에서는 몇 가지 일반적인 사용 사례를 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-123">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="bccfc-124">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="bccfc-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="bccfc-125">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="bccfc-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="bccfc-126">Web Apps</span><span class="sxs-lookup"><span data-stu-id="bccfc-126">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="bccfc-127">SQL Database</span><span class="sxs-lookup"><span data-stu-id="bccfc-127">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="bccfc-128">각 Azure CLI 명령을 사용하는 방법이 설명된 자세한 [참고 자료](/cli/azure/reference-index)도 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-128">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="bccfc-129">이전 버전의 CLI(Azure 클래식 CLI)를 사용하는 경우 계속 사용해도 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-129">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="bccfc-130">그러나 최상의 환경을 위해 Azure CLI의 최신 버전을 사용하도록 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="bccfc-130">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="bccfc-131">두 CLI를 모두 사용하는 경우 `azure`는 클래식 CLI이고 `az`는 최신 CLI라는 사실을 기억하세요.</span><span class="sxs-lookup"><span data-stu-id="bccfc-131">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>

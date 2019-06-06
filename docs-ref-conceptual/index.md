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
ms.openlocfilehash: 0c91b8d49c7854f3963985aa64bbd3c052660f9c
ms.sourcegitcommit: f1031052dd021ebcc253e4b3a5e6b919d862fab2
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2019
ms.locfileid: "64564287"
---
# <a name="azure-command-line-interface-cli"></a><span data-ttu-id="0deb2-103">Azure CLI(명령줄 인터페이스)</span><span class="sxs-lookup"><span data-stu-id="0deb2-103">Azure Command-Line Interface (CLI)</span></span>

<span data-ttu-id="0deb2-104">Azure CLI(명령줄 인터페이스)는 Azure 리소스를 관리하기 위한 Microsoft의 플랫폼 간 명령줄 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="0deb2-104">The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span> <span data-ttu-id="0deb2-105">Azure CLI는 배우기 쉽고, Azure 리소스를 사용하여 맞춤형 자동화를 구축하는 데 적합한 툴입니다.</span><span class="sxs-lookup"><span data-stu-id="0deb2-105">The Azure CLI is easy to learn and the perfect tool for building custom automation that works with Azure resources.</span></span>

| <span data-ttu-id="0deb2-106"><center>![Windows 로고](./media/Windows_logo_-_2012.png)</span><span class="sxs-lookup"><span data-stu-id="0deb2-106"><center>![Windows logo](./media/Windows_logo_-_2012.png)</span></span><br/><span data-ttu-id="0deb2-107">Windows 10</center></span><span class="sxs-lookup"><span data-stu-id="0deb2-107">Windows 10</center></span></span> | <span data-ttu-id="0deb2-108"><center>![Ubuntu 로고](./media/cof_orange_hex.png)</span><span class="sxs-lookup"><span data-stu-id="0deb2-108"><center>![Ubuntu logo](./media/cof_orange_hex.png)</span></span><br/><span data-ttu-id="0deb2-109">Ubuntu 16.04+</center></span><span class="sxs-lookup"><span data-stu-id="0deb2-109">Ubuntu 16.04+</center></span></span> | <span data-ttu-id="0deb2-110"><center>![macOS 로고](./media/Apple_logo_black.png)</span><span class="sxs-lookup"><span data-stu-id="0deb2-110"><center>![macOS logo](./media/Apple_logo_black.png)</span></span><br/><span data-ttu-id="0deb2-111">macOS</center></span><span class="sxs-lookup"><span data-stu-id="0deb2-111">macOS</center></span></span> | <span data-ttu-id="0deb2-112"><center>![Azure Cloud Shell 로고](./media/cloud-check.png)</span><span class="sxs-lookup"><span data-stu-id="0deb2-112"><center>![Azure Cloud Shell logo](./media/cloud-check.png)</span></span><br/><span data-ttu-id="0deb2-113">Azure Cloud Shell</center></span><span class="sxs-lookup"><span data-stu-id="0deb2-113">Azure Cloud Shell</center></span></span> |
|---|---|---|---|
| [<span data-ttu-id="0deb2-114">MSI 설치 관리자 다운로드</span><span class="sxs-lookup"><span data-stu-id="0deb2-114">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows) | [<span data-ttu-id="0deb2-115">Ubuntu 설치 지침</span><span class="sxs-lookup"><span data-stu-id="0deb2-115">Ubuntu install instructions</span></span>](./install-azure-cli-apt.md) | [<span data-ttu-id="0deb2-116">macOS 설치 지침</span><span class="sxs-lookup"><span data-stu-id="0deb2-116">macOS install instructions</span></span>](./install-azure-cli-macos.md) | [<span data-ttu-id="0deb2-117">브라우저에서 Azure Cloud Shell 실행</span><span class="sxs-lookup"><span data-stu-id="0deb2-117">Run in your browser on Azure Cloud Shell</span></span>](https://shell.azure.com) |

[<span data-ttu-id="0deb2-118">모든 지원 되는 설치 플랫폼을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="0deb2-118">See all of the supported installation platforms.</span></span>](./install-azure-cli.md)

## <a name="azure-cli-resources"></a><span data-ttu-id="0deb2-119">Azure CLI 리소스</span><span class="sxs-lookup"><span data-stu-id="0deb2-119">Azure CLI Resources</span></span>

> [!NOTE]
>
> <span data-ttu-id="0deb2-120">스크립트 및 Microsoft 설명서 사이트에 작성된 Azure CLI 예제는 `bash` 셸용입니다.</span><span class="sxs-lookup"><span data-stu-id="0deb2-120">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="0deb2-121">한 줄 예제는 모든 플랫폼에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="0deb2-121">One-line examples will run on any platform.</span></span> <span data-ttu-id="0deb2-122">연속하는 줄을 포함하는 더 긴 예제 (`\`) 또는 변수 할당은 PowerShell을 포함하여 다른 셸에서 작동하도록 수정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0deb2-122">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

| <span data-ttu-id="0deb2-123">시작하기</span><span class="sxs-lookup"><span data-stu-id="0deb2-123">Get started</span></span> | <span data-ttu-id="0deb2-124">Microsoft Learn을 통해 기술 쌓기</span><span class="sxs-lookup"><span data-stu-id="0deb2-124">Build your skills with Microsoft Learn</span></span> | <span data-ttu-id="0deb2-125">문의처</span><span class="sxs-lookup"><span data-stu-id="0deb2-125">Contact Us</span></span> |
|-------------|----------------------------------------|------------|
| [<span data-ttu-id="0deb2-126">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="0deb2-126">Get Started with the Azure CLI</span></span>](get-started-with-azure-cli.md) | [<span data-ttu-id="0deb2-127">Azure CLI로 가상 머신 만들기</span><span class="sxs-lookup"><span data-stu-id="0deb2-127">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/) | [<span data-ttu-id="0deb2-128">기능 요청</span><span class="sxs-lookup"><span data-stu-id="0deb2-128">Request features</span></span>](https://github.com/Azure/azure-cli/issues/new?template=Feature_request.md) |
| [<span data-ttu-id="0deb2-129">GitHub에서 웹 애플리케이션 배포</span><span class="sxs-lookup"><span data-stu-id="0deb2-129">Deploy a web application from GitHub</span></span>](/azure/app-service/scripts/cli-deploy-github?toc=%2fcli%2fazure%2ftoc.json) | [<span data-ttu-id="0deb2-130">CLI를 사용하여 Azure 서비스 제어</span><span class="sxs-lookup"><span data-stu-id="0deb2-130">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/) | [<span data-ttu-id="0deb2-131">StackOverflow에서 도움 받기</span><span class="sxs-lookup"><span data-stu-id="0deb2-131">Get help on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/azure-cli) |
| [<span data-ttu-id="0deb2-132">Postgres 데이터베이스 만들기</span><span class="sxs-lookup"><span data-stu-id="0deb2-132">Create a Postgres database</span></span>](/azure/postgresql/quickstart-create-server-up-azure-cli?toc=%2fcli%2fazure%2ftoc.json) |  [<span data-ttu-id="0deb2-133">Azure Storage에 애플리케이션 연결</span><span class="sxs-lookup"><span data-stu-id="0deb2-133">Connect an application to Azure Storage</span></span>](/learn/modules/connect-an-app-to-azure-storage/) | [<span data-ttu-id="0deb2-134">문제 보고</span><span class="sxs-lookup"><span data-stu-id="0deb2-134">Report issues</span></span>](https://github.com/Azure/azure-cli/issues/new?template=Bug_report.md) |
| [<span data-ttu-id="0deb2-135">Kubernetes 클러스터 만들기</span><span class="sxs-lookup"><span data-stu-id="0deb2-135">Create a Kubernetes cluster</span></span>](/azure/aks/kubernetes-walkthrough?toc=%2fcli%2fazure%2ftoc.json) | [<span data-ttu-id="0deb2-136">더 많은 대화형 학습 보기...</span><span class="sxs-lookup"><span data-stu-id="0deb2-136">More interactive learning...</span></span>](/learn/browse/?products=azure-clis) | |
| [<span data-ttu-id="0deb2-137">가상 머신 만들기</span><span class="sxs-lookup"><span data-stu-id="0deb2-137">Create a virtual machine</span></span>](/cli/azure/azure-cli-vm-tutorial) | | |

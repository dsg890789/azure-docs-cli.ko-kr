---
title: Azure CLI 2.0에 대해 사용 가능한 확장
description: Azure CLI 2.0에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ceca7ed92435ab03b196e60dee37195330f6f3c7
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/28/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a><span data-ttu-id="ee080-103">Azure CLI 2.0에 대해 사용 가능한 확장</span><span class="sxs-lookup"><span data-stu-id="ee080-103">Available extensions for the Azure CLI 2.0</span></span>

<span data-ttu-id="ee080-104">이 문서는 Microsoft에서 제공하고 지원하는 Azure CLI 2.0에 사용할 수 있는 전체 확장 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-104">This article is a complete list of the available extensions for the Azure CLI 2.0 which are offered and supported by Microsoft.</span></span>

<span data-ttu-id="ee080-105">확장 목록도 CLI로부터 직접 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-105">The list of extensions is also available directly from the CLI.</span></span> <span data-ttu-id="ee080-106">가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-106">To get it, run [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):</span></span>

```azurecli
az extension list-available --output table
```

| <span data-ttu-id="ee080-107">이름</span><span class="sxs-lookup"><span data-stu-id="ee080-107">Name</span></span> | <span data-ttu-id="ee080-108">버전</span><span class="sxs-lookup"><span data-stu-id="ee080-108">Version</span></span> | <span data-ttu-id="ee080-109">요약</span><span class="sxs-lookup"><span data-stu-id="ee080-109">Summary</span></span> | <span data-ttu-id="ee080-110">미리 보기</span><span class="sxs-lookup"><span data-stu-id="ee080-110">Preview</span></span> |
|------|---------|---------|---------|
| [<span data-ttu-id="ee080-111">aem</span><span class="sxs-lookup"><span data-stu-id="ee080-111">aem</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-112">0.1.0</span><span class="sxs-lookup"><span data-stu-id="ee080-112">0.1.0</span></span> | <span data-ttu-id="ee080-113">SAP용 Azure 고급 모니터링 확장을 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-113">Manage Azure Enhanced Monitoring Extensions for SAP.</span></span> |  |
| [<span data-ttu-id="ee080-114">alias</span><span class="sxs-lookup"><span data-stu-id="ee080-114">alias</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-115">0.2.0</span><span class="sxs-lookup"><span data-stu-id="ee080-115">0.2.0</span></span> | <span data-ttu-id="ee080-116">명령 별칭을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-116">Support for command aliases.</span></span> |  |
| [<span data-ttu-id="ee080-117">azure-batch-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="ee080-117">azure-batch-cli-extensions</span></span>](https://github.com/Azure/azure-batch-cli-extensions) | <span data-ttu-id="ee080-118">2.1.0</span><span class="sxs-lookup"><span data-stu-id="ee080-118">2.1.0</span></span> | <span data-ttu-id="ee080-119">추가 미리 보기 Azure Batch 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-119">Additional preview Azure Batch commands.</span></span> |  |
| [<span data-ttu-id="ee080-120">azure-cli-iot-ext</span><span class="sxs-lookup"><span data-stu-id="ee080-120">azure-cli-iot-ext</span></span>](https://github.com/azure/azure-iot-cli-extension) | <span data-ttu-id="ee080-121">0.4.1</span><span class="sxs-lookup"><span data-stu-id="ee080-121">0.4.1</span></span> | <span data-ttu-id="ee080-122">Azure IoT Hub, IoT Edge 및 IoT 장치 프로비전 서비스에 대한 데이터 플레인 명령 계층을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-122">Provides the data plane command layer for Azure IoT Hub, IoT Edge and IoT Device Provisioning Service.</span></span> |  |
| [<span data-ttu-id="ee080-123">dns</span><span class="sxs-lookup"><span data-stu-id="ee080-123">dns</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-124">0.0.1</span><span class="sxs-lookup"><span data-stu-id="ee080-124">0.0.1</span></span> | <span data-ttu-id="ee080-125">Azure 사설 DNS 영역 공개 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-125">Support for the Azure Private DNS Public Preview.</span></span> |  |
| [<span data-ttu-id="ee080-126">image-copy-extension</span><span class="sxs-lookup"><span data-stu-id="ee080-126">image-copy-extension</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-127">0.0.5</span><span class="sxs-lookup"><span data-stu-id="ee080-127">0.0.5</span></span> | <span data-ttu-id="ee080-128">영역 간에 이미지를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-128">Copy images from region to region.</span></span> |  |
| [<span data-ttu-id="ee080-129">managementgroups</span><span class="sxs-lookup"><span data-stu-id="ee080-129">managementgroups</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-130">0.1.0</span><span class="sxs-lookup"><span data-stu-id="ee080-130">0.1.0</span></span> | <span data-ttu-id="ee080-131">관리 그룹 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-131">Support for Management Groups preview.</span></span> | <span data-ttu-id="ee080-132">예</span><span class="sxs-lookup"><span data-stu-id="ee080-132">Yes</span></span> |
| [<span data-ttu-id="ee080-133">managementpartner</span><span class="sxs-lookup"><span data-stu-id="ee080-133">managementpartner</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-134">0.1.0</span><span class="sxs-lookup"><span data-stu-id="ee080-134">0.1.0</span></span> | <span data-ttu-id="ee080-135">관리 파트너 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-135">Support for Management Partner preview.</span></span> | <span data-ttu-id="ee080-136">예</span><span class="sxs-lookup"><span data-stu-id="ee080-136">Yes</span></span> |
| [<span data-ttu-id="ee080-137">rdbms</span><span class="sxs-lookup"><span data-stu-id="ee080-137">rdbms</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-138">0.0.4</span><span class="sxs-lookup"><span data-stu-id="ee080-138">0.0.4</span></span> | <span data-ttu-id="ee080-139">Azure MySQL 및 Azure PostgreSQL을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-139">Support for Azure MySQL and Azure PostgreSQL.</span></span> |  |
| [<span data-ttu-id="ee080-140">subscription</span><span class="sxs-lookup"><span data-stu-id="ee080-140">subscription</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-141">0.1.0</span><span class="sxs-lookup"><span data-stu-id="ee080-141">0.1.0</span></span> | <span data-ttu-id="ee080-142">구독 정의 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-142">Support for subscription definitions preview.</span></span> | <span data-ttu-id="ee080-143">예</span><span class="sxs-lookup"><span data-stu-id="ee080-143">Yes</span></span> |
| [<span data-ttu-id="ee080-144">webapp</span><span class="sxs-lookup"><span data-stu-id="ee080-144">webapp</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="ee080-145">0.2.0</span><span class="sxs-lookup"><span data-stu-id="ee080-145">0.2.0</span></span> | <span data-ttu-id="ee080-146">appservice 리소스를 만들고 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="ee080-146">Create and deploy appservice resources.</span></span> | <span data-ttu-id="ee080-147">예</span><span class="sxs-lookup"><span data-stu-id="ee080-147">Yes</span></span> |

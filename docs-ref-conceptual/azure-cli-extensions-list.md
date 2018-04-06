---
title: Azure CLI 2.0에 대해 사용 가능한 확장
description: Azure CLI 2.0에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/02/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e7cf22d1611c224e1d7af351210e12fe0124fad0
ms.sourcegitcommit: 26e0816dad17cc3584d1724493feecf5f5faa1f5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/04/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a><span data-ttu-id="a9510-103">Azure CLI 2.0에 대해 사용 가능한 확장</span><span class="sxs-lookup"><span data-stu-id="a9510-103">Available extensions for the Azure CLI 2.0</span></span>

<span data-ttu-id="a9510-104">이 문서는 Microsoft에서 제공하고 지원하는 Azure CLI 2.0에 사용할 수 있는 전체 확장 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-104">This article is a complete list of the available extensions for the Azure CLI 2.0 which are offered and supported by Microsoft.</span></span>

<span data-ttu-id="a9510-105">확장 목록도 CLI로부터 직접 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-105">The list of extensions is also available directly from the CLI.</span></span> <span data-ttu-id="a9510-106">가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-106">To get it, run [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):</span></span>

```azurecli
az extension list-available --output table
```

| <span data-ttu-id="a9510-107">Name</span><span class="sxs-lookup"><span data-stu-id="a9510-107">Name</span></span> | <span data-ttu-id="a9510-108">버전</span><span class="sxs-lookup"><span data-stu-id="a9510-108">Version</span></span> | <span data-ttu-id="a9510-109">요약</span><span class="sxs-lookup"><span data-stu-id="a9510-109">Summary</span></span> | <span data-ttu-id="a9510-110">미리 보기</span><span class="sxs-lookup"><span data-stu-id="a9510-110">Preview</span></span> |
|------|---------|---------|---------|
| [<span data-ttu-id="a9510-111">aem</span><span class="sxs-lookup"><span data-stu-id="a9510-111">aem</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-112">0.1.1</span><span class="sxs-lookup"><span data-stu-id="a9510-112">0.1.1</span></span> | <span data-ttu-id="a9510-113">SAP용 Azure 고급 모니터링 확장을 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-113">Manage Azure Enhanced Monitoring Extensions for SAP.</span></span> |  |
| [<span data-ttu-id="a9510-114">alias</span><span class="sxs-lookup"><span data-stu-id="a9510-114">alias</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-115">0.3.0</span><span class="sxs-lookup"><span data-stu-id="a9510-115">0.3.0</span></span> | <span data-ttu-id="a9510-116">명령 별칭을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-116">Support for command aliases.</span></span> | <span data-ttu-id="a9510-117">예</span><span class="sxs-lookup"><span data-stu-id="a9510-117">Yes</span></span> |
| [<span data-ttu-id="a9510-118">azure-batch-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="a9510-118">azure-batch-cli-extensions</span></span>](https://github.com/Azure/azure-batch-cli-extensions) | <span data-ttu-id="a9510-119">2.1.0</span><span class="sxs-lookup"><span data-stu-id="a9510-119">2.1.0</span></span> | <span data-ttu-id="a9510-120">추가 미리 보기 Azure Batch 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-120">Additional preview Azure Batch commands.</span></span> |  |
| [<span data-ttu-id="a9510-121">azure-cli-iot-ext</span><span class="sxs-lookup"><span data-stu-id="a9510-121">azure-cli-iot-ext</span></span>](https://github.com/azure/azure-iot-cli-extension) | <span data-ttu-id="a9510-122">0.4.1</span><span class="sxs-lookup"><span data-stu-id="a9510-122">0.4.1</span></span> | <span data-ttu-id="a9510-123">Azure IoT Hub, IoT Edge 및 IoT 장치 프로비전 서비스에 대한 데이터 플레인 명령 계층을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-123">Provides the data plane command layer for Azure IoT Hub, IoT Edge and IoT Device Provisioning Service.</span></span> |  |
| [<span data-ttu-id="a9510-124">dns</span><span class="sxs-lookup"><span data-stu-id="a9510-124">dns</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-125">0.0.2</span><span class="sxs-lookup"><span data-stu-id="a9510-125">0.0.2</span></span> | <span data-ttu-id="a9510-126">Azure 사설 DNS 영역 공개 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-126">Support for the Azure Private DNS Public Preview.</span></span> |  |
| [<span data-ttu-id="a9510-127">image-copy-extension</span><span class="sxs-lookup"><span data-stu-id="a9510-127">image-copy-extension</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-128">0.0.5</span><span class="sxs-lookup"><span data-stu-id="a9510-128">0.0.5</span></span> | <span data-ttu-id="a9510-129">영역 간에 이미지를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-129">Copy images from region to region.</span></span> |  |
| [<span data-ttu-id="a9510-130">managementgroups</span><span class="sxs-lookup"><span data-stu-id="a9510-130">managementgroups</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-131">0.1.0</span><span class="sxs-lookup"><span data-stu-id="a9510-131">0.1.0</span></span> | <span data-ttu-id="a9510-132">관리 그룹 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-132">Support for Management Groups preview.</span></span> | <span data-ttu-id="a9510-133">예</span><span class="sxs-lookup"><span data-stu-id="a9510-133">Yes</span></span> |
| [<span data-ttu-id="a9510-134">managementpartner</span><span class="sxs-lookup"><span data-stu-id="a9510-134">managementpartner</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-135">0.1.2</span><span class="sxs-lookup"><span data-stu-id="a9510-135">0.1.2</span></span> | <span data-ttu-id="a9510-136">관리 파트너 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-136">Support for Management Partner preview.</span></span> | <span data-ttu-id="a9510-137">예</span><span class="sxs-lookup"><span data-stu-id="a9510-137">Yes</span></span> |
| [<span data-ttu-id="a9510-138">rdbms</span><span class="sxs-lookup"><span data-stu-id="a9510-138">rdbms</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-139">0.0.5</span><span class="sxs-lookup"><span data-stu-id="a9510-139">0.0.5</span></span> | <span data-ttu-id="a9510-140">Azure MySQL 및 Azure PostgreSQL을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-140">Support for Azure MySQL and Azure PostgreSQL.</span></span> |  |
| [<span data-ttu-id="a9510-141">subscription</span><span class="sxs-lookup"><span data-stu-id="a9510-141">subscription</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-142">0.1.1</span><span class="sxs-lookup"><span data-stu-id="a9510-142">0.1.1</span></span> | <span data-ttu-id="a9510-143">구독 정의 미리 보기를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-143">Support for subscription definitions preview.</span></span> | <span data-ttu-id="a9510-144">예</span><span class="sxs-lookup"><span data-stu-id="a9510-144">Yes</span></span> |
| [<span data-ttu-id="a9510-145">webapp</span><span class="sxs-lookup"><span data-stu-id="a9510-145">webapp</span></span>](https://github.com/Azure/azure-cli-extensions) | <span data-ttu-id="a9510-146">0.2.0</span><span class="sxs-lookup"><span data-stu-id="a9510-146">0.2.0</span></span> | <span data-ttu-id="a9510-147">appservice 리소스를 만들고 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="a9510-147">Create and deploy appservice resources.</span></span> | <span data-ttu-id="a9510-148">예</span><span class="sxs-lookup"><span data-stu-id="a9510-148">Yes</span></span> |

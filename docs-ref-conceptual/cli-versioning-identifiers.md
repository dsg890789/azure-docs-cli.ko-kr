---
title: Azure CLI 제품 간의 차이점
description: Azure CLI 제품 명명, 버전 지정 및 업그레이드 방법을 이해합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/12/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 4370616459ad4e466128ff26123c10f55bfdd7d8
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178175"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="09157-103">Azure CLI 제품 간의 차이점</span><span class="sxs-lookup"><span data-stu-id="09157-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="09157-104">2018년 6월 말을 기준으로 Azure CLI 제품 이름에서 명시적 버전 번호가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="09157-105">이 변경은 사용자가 "Azure CLI"를 사용하라는 지시를 받았을 때 설명서에 나타났던 혼동을 제거하는 데 도움이 되지만 참조되는 제품의 버전이 명확하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="09157-106">이전 제품 이름에 익숙한 경우, 변경된 내용은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="09157-107">Azure CLI 버전 2.0 이상은 이제 "Azure CLI"라고만 참조됩니다.</span><span class="sxs-lookup"><span data-stu-id="09157-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="09157-108">이전 Azure CLI 버전(1.x 이하)은 이제 "Azure 클래식 CLI"로 참조됩니다.</span><span class="sxs-lookup"><span data-stu-id="09157-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="09157-109">클래식 Azure CLI로 이름이 변경된 것은 이 도구는 클래식 배포 모델에만 사용될 것을 명시하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="09157-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="09157-110">클래식 CLI는 또한 더 이상 업데이트되거나 유지 관리되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="09157-111">이러한 이유로, 클래식 배포를 이동하여 Azure Resource Manager 모델을 사용하고 사용 가능한 최신 버전의 Azure CLI로 마이그레이션하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="09157-112">여전히 클래식 CLI를 사용할 경우, 다음 문서에서 마이그레이션하는 프로세스에 대해 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09157-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="09157-113">클래식에서 Azure Resource Manager로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="09157-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="09157-114">Azure CLI 설치</span><span class="sxs-lookup"><span data-stu-id="09157-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* [<span data-ttu-id="09157-115">클래식 Azure CLI에서 Azure CLI로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="09157-115">Migrating from Azure classic CLI to Azure CLI</span></span>](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)

---
title: Azure CLI를 사용하여 클라우드를 선택합니다.
description: Azure CLI를 사용하여 여러 클라우드를 만들고, 로그인하고, 관리합니다.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 92910e68a52fad3b3577db1bd01e918b69a895d7
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177711"
---
# <a name="select-clouds-with-the-azure-cli"></a><span data-ttu-id="ee20b-103">Azure CLI를 사용하여 클라우드를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-103">Select clouds with the Azure CLI</span></span> 

<span data-ttu-id="ee20b-104">서로 다른 영역에서 작업하거나 [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/)을 사용할 경우 하나 이상의 클라우드를 사용해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="ee20b-105">Microsoft는 제품 사용에 적용될 수 있는 지역 법을 준수하기 위해 클라우드를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="ee20b-106">이 문서에서는 클라우드에 대한 정보를 얻고 현재 클라우드를 변경하고 새 클라우드를 등록 또는 등록 취소하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="ee20b-107">사용할 수 있는 클라우드 목록</span><span class="sxs-lookup"><span data-stu-id="ee20b-107">List available clouds</span></span>

<span data-ttu-id="ee20b-108">[az cloud list](/cli/azure/cloud#az-cloud-list) 명령을 사용하여 사용 가능한 클라우드를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="ee20b-109">이 명령으로 현재 활성 클라우드, 현재 프로필, 지역별 접미사 및 호스트 이름에 대한 정보를 알 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="ee20b-110">활성 클라우드와 모든 사용 가능한 클라우드 목록을 가져오려면:</span><span class="sxs-lookup"><span data-stu-id="ee20b-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

<span data-ttu-id="ee20b-111">현재 활성 클라우드에는 `IsActive` 열에 `True`가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="ee20b-112">언제든지 하나의 클라우드만 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="ee20b-113">Azure 서비스에 사용하는 엔드포인트를 포함하여 클라우드에 대한 자세한 정보를 알아보려면 `cloud show` 명령을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="ee20b-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switch-the-active-cloud"></a><span data-ttu-id="ee20b-114">활성 클라우드 전환</span><span class="sxs-lookup"><span data-stu-id="ee20b-114">Switch the active cloud</span></span>

<span data-ttu-id="ee20b-115">현재 활성 클라우드를 전환하려면 [az cloud set](/cli/azure/cloud#az-cloud-set) 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-115">To switch the currently active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="ee20b-116">이 명령은 하나의 필수 인수인 클라우드 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="ee20b-117">활성화된 클라우드에 대한 인증이 만료된 경우에 다른 CLI 작업을 수행하기 전에 다시 인증해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="ee20b-118">새로운 클라우드로 처음 전환하는 경우도 활성 구독을 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="ee20b-119">인증에 대한 지침은 [Azure CLI를 사용하여 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ee20b-119">For instructions on authenticating, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span> <span data-ttu-id="ee20b-120">구독 관리에 대한 자세한 내용은 [Azure CLI를 사용하여 Azure 구독 관리](manage-azure-subscriptions-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ee20b-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="ee20b-121">새 클라우드를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-121">Register a new cloud</span></span>

<span data-ttu-id="ee20b-122">Azure Stack에 대한 사용자 고유의 엔드포인트가 있는 경우 새 클라우드를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="ee20b-123">클라우드를 만들려면 [az cloud register](/cli/azure/cloud#az-cloud-register) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-123">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="ee20b-124">이 명령에는 이름 및 서비스 엔드포인트 집합이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-124">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="ee20b-125">Azure Stack과 함께 사용할 클라우드를 등록하는 방법에 대해 알아보려면 [Azure Stack에서 Azure CLI와 함께 API 버전 프로필 사용](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ee20b-125">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="ee20b-126">중국, 미국 정부 또는 독일 지역의 경우 클라우드를 등록할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-126">You do don't to register your own cloud for the China, US Government, or German regions.</span></span> <span data-ttu-id="ee20b-127">이들 클라우드는 Microsoft에서 관리하며 기본적으로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-127">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="ee20b-128">사용 가능한 모든 엔드포인트 설정에 대한 자세한 내용은 [에 대한 설명서를 참조하세요`az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="ee20b-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="ee20b-129">클라우드를 등록하더라도 자동으로 해당 클라우드로 전환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-129">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="ee20b-130">`az cloud set` 명령을 사용하여 새로 만든 클라우드를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-130">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="ee20b-131">기존 클라우드 업데이트</span><span class="sxs-lookup"><span data-stu-id="ee20b-131">Update an existing cloud</span></span>

<span data-ttu-id="ee20b-132">권한이 있는 경우 기존 클라우드를 업데이트할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="ee20b-133">클라우드를 업데이트하면 다른 Azure 서비스 프로필로 전환하거나 연결 엔드포인트를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-133">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="ee20b-134">`az cloud register`와 동일한 인수를 사용하여 [az cloud update](/cli/azure/cloud#az-cloud-update) 명령으로 클라우드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-134">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="ee20b-135">클라우드 등록 취소</span><span class="sxs-lookup"><span data-stu-id="ee20b-135">Unregister a cloud</span></span>

<span data-ttu-id="ee20b-136">만든 클라우드가 더 이상 필요하지 않으면 [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) 명령을 사용하여 등록을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee20b-136">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```

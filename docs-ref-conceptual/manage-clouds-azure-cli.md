---
title: "Azure CLI 2.0을 사용하여 여러 클라우드 관리"
description: "Azure CLI 2.0을 사용하여 여러 클라우드를 만들고, 로그인하고, 관리합니다."
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: ee6b1b6b1e611229ba6e6e0c4b2ca2de6f7ceaee
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="6bc15-103">Azure CLI 2.0을 사용하여 여러 클라우드 관리</span><span class="sxs-lookup"><span data-stu-id="6bc15-103">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="6bc15-104">서로 다른 영역에서 작업하거나 [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/)을 사용할 경우 하나 이상의 클라우드를 사용해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="6bc15-105">Microsoft는 제품 사용에 적용될 수 있는 지역 법을 준수하기 위해 클라우드를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="6bc15-106">이 문서에서는 계정에서 사용할 수 있는 클라우드에 대한 정보를 얻고 현재 클라우드를 변경하고 Azure Stack에서 사용할 새 클라우드를 등록 또는 등록 취소하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-106">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="6bc15-107">클라우드 나열</span><span class="sxs-lookup"><span data-stu-id="6bc15-107">Listing clouds</span></span>

<span data-ttu-id="6bc15-108">[cloud list](/cli/azure/cloud#list) 명령을 사용하여 사용 가능한 클라우드를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-108">You can list available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="6bc15-109">이렇게 하면 현재 활성 클라우드, 현재 프로필, 지역별 접미사 및 호스트 이름에 대한 정보를 알 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-109">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="6bc15-110">활성 클라우드와 모든 사용 가능한 클라우드 목록을 가져오려면:</span><span class="sxs-lookup"><span data-stu-id="6bc15-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli
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

<span data-ttu-id="6bc15-111">현재 활성 클라우드에는 `IsActive` 열에 `True`가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="6bc15-112">언제든지 하나의 클라우드만 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="6bc15-113">Azure 서비스에 사용하는 끝점을 포함하여 클라우드에 대한 자세한 정보를 알아보려면 `cloud show` 명령을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="6bc15-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli
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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="6bc15-114">활성 클라우드 전환</span><span class="sxs-lookup"><span data-stu-id="6bc15-114">Switching the active cloud</span></span>

<span data-ttu-id="6bc15-115">현재 활성 클라우드를 전환하려면 [cloud set](/cli/azure/cloud#set) 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-115">To switch the currently active cloud, run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="6bc15-116">이 명령은 하나의 필수 인수인 클라우드 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="6bc15-117">활성화된 클라우드에 대한 인증이 만료된 경우에 다른 CLI 작업을 수행하기 전에 다시 인증해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="6bc15-118">새로운 클라우드로 처음 전환하는 경우도 활성 구독을 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="6bc15-119">인증에 대한 지침은 [Azure CLI 2.0을 사용하여 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6bc15-119">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="6bc15-120">구독 관리에 대한 자세한 내용은 [Azure CLI 2.0을 사용하여 Azure 구독 관리](manage-azure-subscriptions-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6bc15-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="6bc15-121">클라우드 등록</span><span class="sxs-lookup"><span data-stu-id="6bc15-121">Register a cloud</span></span>

<span data-ttu-id="6bc15-122">Azure Stack에 대한 사용자 고유의 끝점이 있는 경우 새 클라우드를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="6bc15-123">클라우드를 만들려면 [cloud register](/cli/azure/cloud#register) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-123">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="6bc15-124">이 명령에는 이름 그리고 연관된 끝점이 있는 기능 집합이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-124">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="6bc15-125">Azure Stack과 함께 사용할 클라우드를 등록하는 방법에 대해 알아보려면 [Azure Stack과 함께 사용할 CLI 설치 및 구성](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6bc15-125">To learn how to register a cloud for use with Azure Stack, see [Install and configure CLI for use with Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span></span>

<span data-ttu-id="6bc15-126">중국, 미국 정부 또는 독일 지역의 경우 클라우드를 등록할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-126">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="6bc15-127">이들 지역은 Microsoft에서 관리하며 기본적으로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-127">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="6bc15-128">사용 가능한 모든 끝점 설정에 대한 자세한 내용은 [에 대한  설명서를 참조하세요`az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span><span class="sxs-lookup"><span data-stu-id="6bc15-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span></span>

<span data-ttu-id="6bc15-129">클라우드를 등록하더라도 자동으로 해당 클라우드로 전환되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-129">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="6bc15-130">위에서 설명한 대로 `az cloud set` 명령을 사용하여 새로 만든 클라우드를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-130">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="6bc15-131">기존 클라우드 업데이트</span><span class="sxs-lookup"><span data-stu-id="6bc15-131">Update an existing cloud</span></span>

<span data-ttu-id="6bc15-132">권한이 있는 경우 기존 클라우드를 업데이트할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="6bc15-133">다른 Azure 프로필로 전환하거나 끝점을 추가하거나 끝점을 변경해야 하는 경우 이를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-133">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="6bc15-134">`az cloud register`과 동일한 인수를 사용하여 `az cloud update` 명령으로 이 작업을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-134">You do this with the `az cloud update` command, which takes the same arguments as `az cloud register`.</span></span> <span data-ttu-id="6bc15-135">자세한 내용은 [의  설명서를 참조하세요`az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span><span class="sxs-lookup"><span data-stu-id="6bc15-135">For more information, see the [documentation for `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="6bc15-136">클라우드 등록 취소</span><span class="sxs-lookup"><span data-stu-id="6bc15-136">Unregister a cloud</span></span>

<span data-ttu-id="6bc15-137">등록한 클라우드가 더 이상 필요하지 않으면 [cloud unregister](/cli/azure/cloud#unregister) 명령을 사용하여 등록을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6bc15-137">If you no longer require a registered cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

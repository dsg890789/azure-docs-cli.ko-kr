---
title: "Azure CLI 2.0을 사용하여 Azure 구독 관리"
description: "Linux, Mac 또는 Windows에서 Azure CLI 2.0을 사용하여 Azure 구독을 관리합니다."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 9f03e52fa72a8dbd5753904839a833db01ffb59b
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="4ad6c-103">여러 Azure 구독 관리</span><span class="sxs-lookup"><span data-stu-id="4ad6c-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="4ad6c-104">대부분의 Azure 사용자는 단일 구독만 가집니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="4ad6c-105">그러나, 사용자가 여러 조직에 속해 있거나 또는 여러 그룹에 걸친 특정 리소스에 액세스하기 위해 조직이 분할된 경우 Azure 내에서 여러 구독을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="4ad6c-106">CLI를 사용하여 여러 구독을 쉽게 관리할 수 있으며, 구독을 선택하여 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="4ad6c-107">테넌트, 사용자 및 구독</span><span class="sxs-lookup"><span data-stu-id="4ad6c-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="4ad6c-108">Azure 내에서 테넌트, 사용자 및 구독 간의 차이에 대해 약간의 혼동이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="4ad6c-109">일반적으로 _테넌트_는 전체 조직을 포괄하는 Azure Active Directory 엔터티입니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="4ad6c-110">이 테넌트에는 하나 이상의 _구독_ 및 _사용자_가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="4ad6c-111">사용자는 개인이며, 소속된 조직인 테넌트 하나와만 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="4ad6c-112">사용자는 Azure에 로그인하여 리소스를 제공하고 사용하는 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="4ad6c-113">사용자는 Azure를 포함하여 클라우드 서비스를 사용하기로 Microsoft와 계약한 여러 _구독_에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="4ad6c-114">모든 리소스가 구독과 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="4ad6c-115">테넌트, 사용자 및 구독 간의 차이점에 대한 자세한 내용은 [Azure 클라우드 용어 사전](/azure/azure-glossary-cloud-terminology)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="4ad6c-116">새 구독을 Azure Active Directory 테넌트에 추가하는 방법을 알아보려면 [Azure 구독을 Azure Active Directory에 추가하는 방법](/azure/active-directory/active-directory-how-subscriptions-associated-directory)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="4ad6c-117">여러 구독 작업</span><span class="sxs-lookup"><span data-stu-id="4ad6c-117">Working with multiple subscriptions</span></span>

<span data-ttu-id="4ad6c-118">구독에 포함된 리소스에 액세스하려면 활성 구독을 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-118">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="4ad6c-119">모든 구독 작업은 `az account` 명령을 통해 수행되며, 이 명령은 구독이 나타내는 서비스 계약을 참조하지만 개인 계정을 참조하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-119">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="4ad6c-120">사용 가능한 구독에 대한 작업을 시작하려면 계정에서 사용할 수 있는 목록을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-120">To start working with your available subscriptions, get a list of those available in your account:</span></span>

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

<span data-ttu-id="4ad6c-121">활성 구독을 변경하려면 `az account set`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-121">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="4ad6c-122">구독 ID 또는 구독 이름을 사용하여 구독을 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ad6c-122">You can use either the subscription ID or the subscription name to select the subscription.</span></span>

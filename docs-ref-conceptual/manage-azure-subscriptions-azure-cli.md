---
title: Azure CLI를 사용하여 Azure 구독을 관리합니다.
description: Azure CLI를 사용하여 Azure 구독을 관리합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.product: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 37ef0c1d7cca90c99aa6f832c6dc6dc29a1806a3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516201"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="f84e8-103">여러 Azure 구독 사용</span><span class="sxs-lookup"><span data-stu-id="f84e8-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="f84e8-104">대부분의 Azure 사용자는 단일 구독만 가집니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="f84e8-105">그러나, 사용자가 여러 조직에 속해 있거나 또는 여러 그룹에 걸친 특정 리소스에 액세스하기 위해 조직이 분할된 경우 Azure 내에서 여러 구독을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="f84e8-106">CLI는 전역적으로 그리고 명령 당 구독을 선택하는 것을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="f84e8-107">구독, 청구 및 비용 관리에 대한 자세한 내용은 [청구 및 비용 관리 설명서](/azure/billing/)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f84e8-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="f84e8-108">테넌트, 사용자 및 구독</span><span class="sxs-lookup"><span data-stu-id="f84e8-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="f84e8-109">Azure 내에서 테넌트, 사용자 및 구독 간의 차이에 대해 약간의 혼동이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="f84e8-110">_테넌트_는 전체 조직을 포괄하는 Azure Active Directory 엔터티입니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="f84e8-111">이 테넌트에는 하나 이상의 _구독_ 및 _사용자_가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="f84e8-112">사용자는 개인이며 소속된 조직인 테넌트 하나와만 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="f84e8-113">사용자는 Azure에 로그인하여 리소스를 생성, 관리, 사용하는 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="f84e8-114">사용자는 Azure를 포함하여 클라우드 서비스를 사용하기로 Microsoft와 계약한 여러 _구독_에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="f84e8-115">모든 리소스가 구독과 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="f84e8-116">테넌트, 사용자 및 구독 간의 차이점에 대한 자세한 내용은 [Azure 클라우드 용어 사전](/azure/azure-glossary-cloud-terminology)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f84e8-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="f84e8-117">새 구독을 Azure Active Directory 테넌트에 추가하는 방법을 알아보려면 [Azure 구독을 Azure Active Directory에 추가하는 방법](/azure/active-directory/active-directory-how-subscriptions-associated-directory)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f84e8-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="f84e8-118">특정 테넌트에 로그인하는 방법을 알아보려면 [Azure CLI로 로그인](/cli/azure/authenticate-azure-cli)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-118">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="f84e8-119">활성 구독 변경</span><span class="sxs-lookup"><span data-stu-id="f84e8-119">Change the active subscription</span></span>

<span data-ttu-id="f84e8-120">구독을 위해 리소스에 액세스하려면, 활성 구독을 전환하거나 `--subscription` 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-120">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="f84e8-121">모든 명령에 대한 구독을 전환하는 작업은 [az 계정 집합](/cli/azure/account#az-account-set)을 사용하여 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-121">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="f84e8-122">활성 구독을 전환하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-122">To switch your active subscription:</span></span>

1. <span data-ttu-id="f84e8-123">[az account list](/cli/azure/account#az-account-list) 명령을 사용하여 구독 리스트를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-123">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="f84e8-124">전환하려고 하는 구독 ID 또는 이름으로 `az account set`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-124">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="f84e8-125">다른 구독을 사용하여 단일 명령만을 실행하려면 `--subscription` 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f84e8-125">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="f84e8-126">이 인수는 구독 ID 또는 구독 이름을 사용합니다:</span><span class="sxs-lookup"><span data-stu-id="f84e8-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

---
title: "Azure CLI 2.0을 사용하여 여러 클라우드 관리"
description: "Azure CLI 2.0을 사용하여 여러 클라우드를 생성, 로그인 및 관리합니다."
keywords: "Azure CLI 2.0, Azure, 클라우드, 데이터 센터, 정부, 지역, 중국, 독일"
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="a211c-104">Azure CLI 2.0을 사용하여 여러 클라우드 관리</span><span class="sxs-lookup"><span data-stu-id="a211c-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="a211c-105">Azure와 관련된 여러 구독이 있는 경우 둘 이상의 클라우드를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="a211c-106">각 클라우드마다 자체의 연결된 끝점과 기능을 갖추고 있으며, 종종 서로 다른 데이터 보호 표준 또는 요구 사항이 있는 특정 지역과 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="a211c-107">여러 클라우드를 효과적으로 사용하려면 현재 활성 중인 클라우드 간에 전환할 수 있어야 하고 새 클라우드를 만들 수도 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="a211c-108">클라우드 나열</span><span class="sxs-lookup"><span data-stu-id="a211c-108">Listing clouds</span></span>

<span data-ttu-id="a211c-109">[cloud list](/cli/azure/cloud#list) 명령을 사용하여 사용 가능한 클라우드를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="a211c-110">이렇게 하면 현재 활성 클라우드와 현재 프로필을 알려주며, 국가별 접미사 및 호스트 이름에 대한 정보를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="a211c-111">사용 가능한 클라우드와 현재 활성 클라우드의 목록을 가져오려면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-111">To get a list of the available clouds and the currently active one:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="a211c-112">활성 클라우드 전환</span><span class="sxs-lookup"><span data-stu-id="a211c-112">Switching the active cloud</span></span>

<span data-ttu-id="a211c-113">현재 활성 클라우드를 전환하려면 [cloud set](/cli/azure/cloud#set) 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="a211c-114">이 명령은 하나의 필수 인수인 클라우드 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="a211c-115">활성 클라우드에 대해 인증한 적이 없는 경우 먼저 활성 클라우드에 인증하여 다른 CLI 작업을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="a211c-116">인증에 대한 지침은 [Azure CLI 2.0을 사용하여 로그인](/cli/azure/authenticate-azure-cli)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a211c-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="a211c-117">클라우드 등록 또는 등록 취소</span><span class="sxs-lookup"><span data-stu-id="a211c-117">Register or unregister a cloud</span></span>

<span data-ttu-id="a211c-118">사용자 고유의 끝점이 있거나 다른 프로필이 필요한 경우 새 클라우드를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="a211c-119">클라우드를 만들려면 [cloud register](/cli/azure/cloud#register) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="a211c-120">이 명령에는 이름 및 선택적으로 기능 및 끝점 지정 집합이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="a211c-121">특정 프로필을 사용하여 리소스 관리자에 대한 특수 끝점이 있는 클라우드를 만들려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="a211c-122">이렇게 하면 클라우드를 만들지만 자동으로 선택하지 _않습니다_.</span><span class="sxs-lookup"><span data-stu-id="a211c-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="a211c-123">만든 클라우드가 더 이상 필요하지 않으면 [cloud unregister](/cli/azure/cloud#unregister) 명령을 사용하여 등록을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a211c-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```


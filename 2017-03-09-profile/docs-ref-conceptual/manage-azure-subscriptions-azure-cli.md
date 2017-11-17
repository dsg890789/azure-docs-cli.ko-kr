---
title: "Azure CLI 2.0을 사용하여 Azure 구독 관리"
description: "Linux, Mac 또는 Windows에서 Azure CLI 2.0을 사용하여 Azure 구독을 관리합니다."
keywords: "Azure CLI 2.0, Linux, Mac, Windows, OS X, 구독"
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: c3538077e05d61f3c40880bb8b804226eb99dc85
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="a72e3-104">여러 Azure 구독 관리</span><span class="sxs-lookup"><span data-stu-id="a72e3-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="a72e3-105">Azure를 처음 접하는 분들은 아마도 구독을 하나만 갖고 계실 것입니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="a72e3-106">하지만 한동안 Azure를 사용해 오신 분들 중에는 Azure 구독을 여러 개 만든 분도 있을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="a72e3-107">구독을 여러 개 만든 분들은 특정 구독에 대해 명령을 실행하도록 Azure CLI 2.0을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="a72e3-108">계정의 모든 구독 목록을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="a72e3-109">기본 구독을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-109">Set the default.</span></span>
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

<span data-ttu-id="a72e3-110">`az account list --output table` 명령을 다시 실행하여 변경 내용을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-110">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="a72e3-111">기본 구독을 설정한 이후부터는 모든 Azure CLI 명령이 기본 구독에 대해 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72e3-111">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>
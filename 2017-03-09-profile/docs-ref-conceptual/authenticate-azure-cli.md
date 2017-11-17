---
title: "Azure CLI 2.0으로 로그인"
description: "Linux, Mac 또는 Windows에서 Azure 2.0 CLI로 로그인합니다."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: fea893ebd55811527e0e92375ffc081a52cdbb57
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="log-in-with-azure-cli-20"></a><span data-ttu-id="23e0e-104">Azure CLI 2.0으로 로그인</span><span class="sxs-lookup"><span data-stu-id="23e0e-104">Log in with Azure CLI 2.0</span></span>

<span data-ttu-id="23e0e-105">Azure CLI를 사용하여 로그인하고 인증하는 여러 방법이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-105">There are several ways to log in and authenticate with the Azure CLI.</span></span> <span data-ttu-id="23e0e-106">가장 간단하게 시작하는 방법은 브라우저를 통해 대화형으로 로그인하거나 명령줄에서 로그인하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-106">The simplest way to get started is to log in interactively through your browser, or to log in at the command line.</span></span> <span data-ttu-id="23e0e-107">리소스를 조작하는 데 사용할 수 있는 비 대화형 계정을 만드는 방법을 제공하는 서비스 주체를 사용할 것을 권장합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-107">Our recommended approach is to use service principals, which provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="23e0e-108">서비스 주체에게 필요한 접근 권한만 부여하여 자동화 스크립트를 훨씬 안전하게 보호할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-108">By granting just the appropriate permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="23e0e-109">CLI를 사용하여 실행하는 명령은 기본 구독에 대해 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-109">Commands that you run with the CLI are run against your default subscription.</span></span>  <span data-ttu-id="23e0e-110">둘 이상의 구독이 있는 경우 [기본 구독을 확인](manage-azure-subscriptions-azure-cli.md)하고 적절하게 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-110">If you have more than one subscription, you may want to [confirm your default subscription](manage-azure-subscriptions-azure-cli.md) and change it appropriately.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="23e0e-111">대화형 로그인</span><span class="sxs-lookup"><span data-stu-id="23e0e-111">Interactive log-in</span></span>

<span data-ttu-id="23e0e-112">웹 브라우저에서 대화형으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-112">Log in interactively from your web browser.</span></span>

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a><span data-ttu-id="23e0e-113">명령 줄</span><span class="sxs-lookup"><span data-stu-id="23e0e-113">Command line</span></span>

<span data-ttu-id="23e0e-114">명령줄에 자격 증명을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-114">Provide your credentials on the command line.</span></span>

> [!Note]
> <span data-ttu-id="23e0e-115">이 접근 방식은 Microsoft 계정 또는 2단계 인증을 사용하는 계정에서는 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-115">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurecli
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a><span data-ttu-id="23e0e-116">서비스 주체로 로그인</span><span class="sxs-lookup"><span data-stu-id="23e0e-116">Logging in with a service principal</span></span>

<span data-ttu-id="23e0e-117">서비스 주체는 Azure Active Directory를 사용하여 규칙을 적용할 수 있는 사용자 계정과 비슷합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-117">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span>
<span data-ttu-id="23e0e-118">리소스를 조작하는 스크립트 또는 응용 프로그램에서 Azure 리소스 사용을 보호하는 가장 좋은 방법은 서비스 주체를 사용하여 인증하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-118">Authenticating with a service principal is the best way to secure the usage of your Azure resources from either your scripts or applications that manipulate resources.</span></span>
<span data-ttu-id="23e0e-119">`az role` 명령 집합을 통해 사용자에게 줄 역할을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-119">You define the roles you want your users to have via the `az role` set of commands.</span></span>
<span data-ttu-id="23e0e-120">[az 역할 참조 문서](https://docs.microsoft.com/cli/azure/role.md)에서 서비스 주체 역할의 자세한 내용과 예제를 살펴볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-120">You can learn more and see examples of service principal roles in our [az role reference articles](https://docs.microsoft.com/cli/azure/role.md).</span></span>

1. <span data-ttu-id="23e0e-121">아직 서비스 주체가 없는 경우 [하나 만듭니다](create-an-azure-service-principal-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="23e0e-121">If you don't already have a service principal, [create one](create-an-azure-service-principal-azure-cli.md).</span></span>

1. <span data-ttu-id="23e0e-122">서비스 주체로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-122">Log in with the service principal.</span></span>

   ```azurecli
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   <span data-ttu-id="23e0e-123">테넌트를 가져오려면 대화형으로 로그인한 다음 구독에서 tenantId를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="23e0e-123">To get your tenant, log in interactively and then get the tenantId from your subscription.</span></span>

   ```azurecli
   az login
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```
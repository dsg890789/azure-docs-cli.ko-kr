---
title: "Azure CLI 2.0을 사용하여 Azure 서비스 주체 만들기"
description: "Azure CLI 2.0을 사용하여 앱 또는 서비스의 서비스 주체를 만드는 방법을 알아봅니다."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 10/12/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: a6ad5611f3e507b65e160122c87e22ec44546588
ms.sourcegitcommit: e8fe15e4f7725302939d726c75ba0fb3cad430be
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/27/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="daa22-104">Azure CLI 2.0을 사용하여 Azure 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="daa22-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="daa22-105">Azure CLI 2.0을 사용하여 앱 또는 서비스를 관리하려는 경우 고유한 자격 증명 대신 AAD(Azure Active Directory) 서비스 주체에서 실행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="daa22-106">이 토픽에서는 Azure CLI 2.0을 사용하여 보안 주체를 만드는 과정을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="daa22-107">Azure Portal을 통해 서비스 주체를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="daa22-108">자세한 내용은 [포털을 사용하여 리소스에 액세스할 수 있는 Active Directory 응용 프로그램 및 서비스 주체 만들기](/azure/azure-resource-manager/resource-group-create-service-principal-portal)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="daa22-109">'서비스 주체'란?</span><span class="sxs-lookup"><span data-stu-id="daa22-109">What is a 'service principal'?</span></span>

<span data-ttu-id="daa22-110">Azure 서비스 주체는 특정 Azure 리소스에 액세스하기 위해 사용자가 만든 앱, 서비스 및 자동화 도구에서 사용하는 보안 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="daa22-111">특정한 역할이 있는 '사용자 ID'(로그인과 암호 또는 인증서)이며 리소스에 액세스하기 위해 엄격하게 제어됩니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="daa22-112">일반 사용자 ID와 달리 특정 작업만을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="daa22-113">해당 관리 작업을 수행하는 데 필요한 최소 사용 권한 수준을 부여하는 경우 보안이 향상됩니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="daa22-114">Azure CLI 2.0은 암호 기반 인증 자격 증명 및 인증서 자격 증명을 만들도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-114">Azure CLI 2.0 supports the creation of password-based authentication credentials and certificate credentials.</span></span> <span data-ttu-id="daa22-115">이 항목에서는 두 가지 자격 증명을 다룹니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-115">In this topic, we cover both types of credentials.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="daa22-116">고유한 사용 권한 수준 확인</span><span class="sxs-lookup"><span data-stu-id="daa22-116">Verify your own permission level</span></span>

<span data-ttu-id="daa22-117">먼저 Azure Active Directory와 Azure 구독에 대한 충분한 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="daa22-118">특히, Active Directory에서 앱을 만들고 서비스 주체에 역할을 할당할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="daa22-119">계정에 적절한 사용 권한이 있는지를 확인하는 가장 쉬운 방법은 포털을 통하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="daa22-120">[포털에서 필요한 사용 권한 확인](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="daa22-121">응용 프로그램에 대한 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="daa22-121">Create a service principal for your application</span></span>

<span data-ttu-id="daa22-122">서비스 주체를 만들 앱을 식별하려면 다음 중 하나가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="daa22-123">예제의 "MyDemoWebApp"처럼 배포된 앱의 고유한 이름 또는 URI</span><span class="sxs-lookup"><span data-stu-id="daa22-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="daa22-124">응용 프로그램 ID, 배포된 앱/서비스/개체와 연결된 고유 GUID</span><span class="sxs-lookup"><span data-stu-id="daa22-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="daa22-125">이러한 값은 서비스 주체를 만들 때 응용 프로그램을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="daa22-126">응용 프로그램에 대한 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="daa22-126">Get information about your application</span></span>

<span data-ttu-id="daa22-127">`az ad app list`를 사용하여 응용 프로그램에 대한 ID 정보를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-127">Get identity information about your application with the `az ad app list`.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

<span data-ttu-id="daa22-128">`--display-name` 옵션은 반환된 앱 목록을 필터링하여 `displayName`이 MyDemoWebApp으로 시작하는 앱만 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-a-service-principal-with-a-password"></a><span data-ttu-id="daa22-129">암호를 사용하여 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="daa22-129">Create a service principal with a password</span></span>

<span data-ttu-id="daa22-130">[az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) 및 `--password` 매개 변수를 사용하여 암호를 가진 서비스 주체를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--password` parameter to create the service principal with a password.</span></span> <span data-ttu-id="daa22-131">역할 또는 범위를 제공하지 않으면 현재 구독의 **참가자** 역할을 기본적으로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-131">When you do not provide a role or scope, it defaults to the **Contributor** role for the current subscription.</span></span> <span data-ttu-id="daa22-132">`--password` 또는 `--cert` 매개 변수 중 하나를 사용하지 않고 서비스 주체를 만드는 경우 암호 인증을 사용하고 암호를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-132">If you create a service principal without using either the `--password` or `--cert` parameter, password authentication is used and a password is generated for you.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
``` 

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING] 
 > <span data-ttu-id="daa22-133">안전하지 않은 암호를 만들지 마세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-133">Don't create an insecure password.</span></span>  <span data-ttu-id="daa22-134">[Azure AD 암호 규칙 및 제한 사항](/azure/active-directory/active-directory-passwords-policy) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-134">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="create-a-service-principal-with-a-self-signed-certificate"></a><span data-ttu-id="daa22-135">자체 서명된 인증서를 사용하여 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="daa22-135">Create a service principal with a self-signed certificate</span></span>

<span data-ttu-id="daa22-136">[az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) 및 `--create-cert` 매개 변수를 사용하여 자체 서명된 인증서를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-136">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--create-cert` parameter to create a self-signed certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --create-cert
```

```json
{
  "appId": "c495db57-82e0-4e2e-9369-069dff176858",
  "displayName": "azure-cli-2017-10-12-22-15-38",
  "fileWithCertAndPrivateKey": "<path>/<file-name>.pem",
  "name": "http://MyDemoWebApp",
  "password": null,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="daa22-137">`fileWithCertAndPrivateKey` 응답의 값을 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-137">Copy the value of the `fileWithCertAndPrivateKey` response.</span></span> <span data-ttu-id="daa22-138">이 항목은 인증에 사용되는 인증서 파일입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-138">This is the certificate file which will be used for authentication.</span></span>

<span data-ttu-id="daa22-139">인증서를 사용할 때 더 많은 옵션은 [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-139">For more options when using certificates, see [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="daa22-140">서비스 주체에 대한 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="daa22-140">Get information about the service principal</span></span>

```azurecli-interactive
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="daa22-141">서비스 주체를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="daa22-141">Sign in using the service principal</span></span>

<span data-ttu-id="daa22-142">이제 `az ad sp show`의 *appId* 및 *암호*나 생성된 인증서의 경로를 사용하여 앱에 새로운 서비스 주체로 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-142">You can now log in as the new service principal for your app using the *appId* from `az ad sp show`, and either the *password* or the path to the created certificate.</span></span>  <span data-ttu-id="daa22-143">`az ad sp create-for-rbac` 결과에서 *테넌트* 값을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-143">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password-or-path-to-cert} --tenant {tenant}
``` 

<span data-ttu-id="daa22-144">성공적으로 로그온하면 이 출력이 표시될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-144">You will see this output after a successful sign-on:</span></span>

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

<span data-ttu-id="daa22-145">앱을 실행하기 위한 자격 증명으로 `id`, `password` 및 `tenant` 값을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-145">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="daa22-146">역할 관리</span><span class="sxs-lookup"><span data-stu-id="daa22-146">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="daa22-147">Azure 역할 기반 Access Control(RBAC)은 사용자 및 서비스 주체에 대한 역할을 정의하고 관리하기 위한 모델입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-147">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="daa22-148">역할에는 그와 관련된 일련의 사용 권한이 있으며 여기서 주체가 읽고 액세스하고 쓰고 관리할 수 있는 리소스를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-148">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="daa22-149">RBAC와 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="daa22-149">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="daa22-150">Azure CLI 2.0은 역할 할당을 관리하는 다음 명령을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-150">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="daa22-151">az 역할 할당 나열</span><span class="sxs-lookup"><span data-stu-id="daa22-151">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="daa22-152">az 역할 할당 만들기</span><span class="sxs-lookup"><span data-stu-id="daa22-152">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="daa22-153">az 역할 할당 삭제</span><span class="sxs-lookup"><span data-stu-id="daa22-153">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="daa22-154">서비스 주체의 기본 역할은 **참가자**입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-154">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="daa22-155">광범위한 사용 권한을 고려하면 앱과 Azure 서비스의 상호 작용을 위한 최상의 선택이 아닐 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-155">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="daa22-156">**판독기** 역할은 더 제한적이며 읽기 전용 액세스에 좋은 선택입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-156">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="daa22-157">역할 관련 사용 권한에 대한 세부 정보를 보거나 Azure Portal을 통해 사용자 지정 레코드를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-157">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="daa22-158">이 예제에서는 **판독기** 역할을 이전 예제에 추가하고 **참가자** 역할을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-158">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="daa22-159">현재 할당된 역할을 나열하여 변경 내용을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-159">Verify the changes by listing the currently assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE] 
> <span data-ttu-id="daa22-160">계정에 역할을 할당할 권한이 없는 경우 오류 메시지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-160">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="daa22-161">이 메시지는 계정에 "/subscriptions/{guid}' 범위에 대해 'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 권한이 없다"는 내용입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-161">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="daa22-162">보안 주체의 자격 증명 변경</span><span class="sxs-lookup"><span data-stu-id="daa22-162">Change the credentials of a security principal</span></span>

<span data-ttu-id="daa22-163">사용 권한을 검토하고 암호를 정기적으로 업데이트하는 것은 좋은 보안 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-163">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="daa22-164">앱이 변경되면 보안 자격 증명을 관리하고 수정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-164">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="daa22-165">서비스 주체 암호 재설정</span><span class="sxs-lookup"><span data-stu-id="daa22-165">Reset a service principal password</span></span>

<span data-ttu-id="daa22-166">`az ad sp reset-credentials` 명령을 사용하여 서비스 주체의 현재 암호를 재설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-166">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

```azurecli-interactive
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="daa22-167">`--password` 옵션을 생략하면 CLI가 안전한 암호를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="daa22-167">The CLI generates a secure password if you leave out the `--password` option.</span></span>

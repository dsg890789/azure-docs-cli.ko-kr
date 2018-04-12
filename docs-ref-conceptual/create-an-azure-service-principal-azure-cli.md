---
title: Azure CLI 2.0에서 Azure 서비스 주체 사용
description: Azure CLI 2.0에서 서비스 주체를 만들고 사용하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/12/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fd615c762f997cb8bd4835d387cd96dd9c475928
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2018
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="1ad5b-103">Azure CLI 2.0을 사용하여 Azure 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="1ad5b-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="1ad5b-104">액세스가 제한된 개별 로그인을 만들려면 서비스 주체를 통해 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="1ad5b-105">서비스 주체는 계정과 연결할 수 있는 별도의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="1ad5b-106">서비스 주체는 자동화해야 하는 응용 프로그램 및 작업을 사용할 때 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="1ad5b-107">이 문서에서는 서비스 주체를 만들기 위한 단계를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="1ad5b-108">서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="1ad5b-108">Create the service principal</span></span>

<span data-ttu-id="1ad5b-109">[az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) 명령을 사용하여 서비스 주체를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="1ad5b-110">서비스 주체 이름은 기존 응용 프로그램 또는 사용자 이름에 연결되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="1ad5b-111">원하는 인증 유형을 선택하여 서비스 주체를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="1ad5b-112">`--password`은(는) 암호 기반 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="1ad5b-113">[Azure Active Directory 암호 규칙 및 제한 사항](/azure/active-directory/active-directory-passwords-policy)에 따라 강력한 암호를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="1ad5b-114">암호를 지정하지 않으면, 자동으로 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="1ad5b-115">`--cert`은(는) 기존 인증서에 대한 인증서 기반 인증(PEM 또는 DER 공용 문자열) 또는 파일 로드를 위한 `@{file}`에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="1ad5b-116">인증서가 Azure Key Vault에 저장되는 것을 나타내기 위해서는 `--keyvault` 인수를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="1ad5b-117">이 경우 `--cert` 값은 Key Vault에 있는 인증서 이름을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

* <span data-ttu-id="1ad5b-118">`--create-cert`은(는) 인증을 위해 _자체 서명된_ 인증서를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="1ad5b-119">`--keyvault` 인수를 추가하면 Azure Key Vault에 인증서를 저장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-119">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

<span data-ttu-id="1ad5b-120">인증 유형을 나타내는 인수가 포함되지 않은 경우, 기본적으로 `--password`이(가) 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-120">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="1ad5b-121">`create-for-rbac` 명령의 출력 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-121">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="1ad5b-122">`appId`, `tenant` 및 `password` 값은 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-122">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="1ad5b-123">`displayName`은(는) 기존 서비스 주체를 검색할 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-123">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="1ad5b-124">계정에 서비스 주체를 만들기 위한 권한이 없는 경우, "권한이 부족하여 작업을 완료할 수 없습니다."가 포함된 오류 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-124">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="1ad5b-125">서비스 주체를 만들려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-125">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="1ad5b-126">서비스 주체 역할 관리</span><span class="sxs-lookup"><span data-stu-id="1ad5b-126">Manage service principal roles</span></span> 

<span data-ttu-id="1ad5b-127">Azure CLI 2.0은 역할 할당 관리를 위해 다음 명령을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-127">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="1ad5b-128">az 역할 할당 나열</span><span class="sxs-lookup"><span data-stu-id="1ad5b-128">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="1ad5b-129">az 역할 할당 만들기</span><span class="sxs-lookup"><span data-stu-id="1ad5b-129">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="1ad5b-130">az 역할 할당 삭제</span><span class="sxs-lookup"><span data-stu-id="1ad5b-130">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="1ad5b-131">서비스 주체의 기본 역할은 **참가자**입니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-131">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="1ad5b-132">이 역할은 Azure 계정에 대한 모든 읽기 및 쓰기 권한을 포함하며, 일반적으로 응용 프로그램에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-132">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="1ad5b-133">**Reader** 역할은 보다 제한적이며, 읽기 전용 액세스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-133">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="1ad5b-134">RBAC(역할 기반 액세스 제어) 및 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-134">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="1ad5b-135">이 예제에서는 **Reader** 역할을 추가하고 **Contributor** 역할을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-135">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="1ad5b-136">역할을 추가해도 이전에 할당된 권한은 변경되지 _않습니다_.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-136">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="1ad5b-137">서비스 주체 권한을 제한할 때는 항상 __Contributor__ 역할을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-137">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="1ad5b-138">변경 사항은 할당된 역할을 나열하여 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-138">The changes can be verified by listing the assigned roles.</span></span>

```azurecli
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="1ad5b-139">계정에 역할 할당 권한이 없으면 계정에 "'/subscriptions/{guid}' 범위에 대해 'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 수 있는 권한이 없습니다." 오류 메시지가 표시됩니다. 역할을 관리하려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-139">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="log-in-using-the-service-principal"></a><span data-ttu-id="1ad5b-140">서비스 주체를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="1ad5b-140">Log in using the service principal</span></span>

<span data-ttu-id="1ad5b-141">Azure CLI 내에서 로그인하여 새로운 서비스 주체의 로그인 및 권한을 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-141">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="1ad5b-142">`appId`, `tenant` 및 자격 증명 값을 사용하여 새로운 서비스 주체로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-142">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="1ad5b-143">사용자가 제공하는 인증 정보는 서비스 주체를 만들 때 암호 또는 인증서를 사용하도록 선택했는지 여부에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-143">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="1ad5b-144">암호를 사용하여 로그인하려면 암호를 인수 매개 변수로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-144">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="1ad5b-145">인증서를 사용하여 로그인하려면 로컬 인증서를 PEM 또는 DER 파일로 사용할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-145">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```
## <a name="reset-credentials"></a><span data-ttu-id="1ad5b-146">자격 증명 다시 설정</span><span class="sxs-lookup"><span data-stu-id="1ad5b-146">Reset credentials</span></span>

<span data-ttu-id="1ad5b-147">서비스 주체의 자격 증명을 잊은 경우에는 [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) 명령으로 다시 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-147">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) command.</span></span> <span data-ttu-id="1ad5b-148">여기에서도 새로운 서비스 주체를 만들 때와 동일한 제한 사항 및 옵션이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad5b-148">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```

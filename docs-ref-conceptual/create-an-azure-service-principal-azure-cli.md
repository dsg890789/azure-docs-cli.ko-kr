---
title: Azure CLI에서 Azure 서비스 주체 사용
description: Azure CLI에서 서비스 주체를 만들고 사용하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6cce8fb47dd2b57180487441055333343fff8330
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805876"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="fad4e-103">Azure CLI를 사용하여 Azure 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="fad4e-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="fad4e-104">액세스가 제한된 개별 로그인을 만들려면 서비스 주체를 통해 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-104">If you want to create a separate sign-in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="fad4e-105">서비스 주체는 계정과 연결할 수 있는 별도의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="fad4e-106">서비스 주체는 자동화해야 하는 애플리케이션 및 작업을 사용할 때 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="fad4e-107">이 문서에서는 서비스 주체를 만들기 위한 단계를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="fad4e-108">서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="fad4e-108">Create the service principal</span></span>

<span data-ttu-id="fad4e-109">[az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) 명령을 사용하여 서비스 주체를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="fad4e-110">서비스 주체 이름은 기존 애플리케이션 또는 사용자 이름에 연결되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="fad4e-111">원하는 인증 유형을 선택하여 서비스 주체를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="fad4e-112">`--password`은(는) 암호 기반 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="fad4e-113">인증 형식을 나타내는 인수가 포함되지 않은 경우 기본적으로 암호가 사용되며 사용자를 위해 암호가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-113">If an argument indicating the authentication type isn't included, --password is used by default, and one is created for you.</span></span> <span data-ttu-id="fad4e-114">암호 기반 인증을 사용하려고 할 때 이 명령을 사용하도록 권장되며, 사용자를 위해 암호가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-114">If you want to use password-based authentication, we recommend using this command, so the password is created for you.</span></span>  

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName 
  ```
  <span data-ttu-id="fad4e-115">사용자를 위해 자동으로 생성되는 암호(보안상의 이유로 권장되지 않음) 대신 직접 암호를 설정하려고 할 때 이 명령을 사용하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-115">If you want to choose the password, instead of it being created for you (which is not recommended, for security reasons), you can use this command.</span></span> <span data-ttu-id="fad4e-116">[Azure Active Directory 암호 규칙 및 제한 사항](/azure/active-directory/active-directory-passwords-policy)에 따라 강력한 암호를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-116">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="fad4e-117">암호 설정 옵션에는 취약한 암호가 설정되거나 암호가 재사용될 가능성이 존재합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-117">The option to choose password leaves the chance of a weak password being chosen or password being re-used.</span></span> <span data-ttu-id="fad4e-118">이 옵션은 Azure CLI의 추후 버전에서는 사용되지 않을 계획입니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-118">This option is planned to be deprecated in a future version of Azure CLI.</span></span> 

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

* <span data-ttu-id="fad4e-119">`--cert`은(는) 기존 인증서에 대한 인증서 기반 인증(PEM 또는 DER 공용 문자열) 또는 파일 로드를 위한 `@{file}`에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-119">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="fad4e-120">인증서가 Azure Key Vault에 저장되는 것을 나타내기 위해서는 `--keyvault` 인수를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-120">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="fad4e-121">이 경우 `--cert` 값은 Key Vault에 있는 인증서 이름을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-121">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="fad4e-122">`--create-cert`은(는) 인증을 위해 _자체 서명된_ 인증서를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-122">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="fad4e-123">`--cert` 인수가 제공되지 않으면 임의의 인증서 이름이 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-123">If the `--cert` argument isn't provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="fad4e-124">`--keyvault` 인수를 추가하면 Azure Key Vault에 인증서를 저장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-124">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="fad4e-125">`--keyvault`을 사용하는 경우 `--cert` 인수 또한 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-125">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="fad4e-126">인증 유형을 나타내는 인수가 포함되지 않은 경우, 기본적으로 `--password`이(가) 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-126">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="fad4e-127">`create-for-rbac` 명령의 JSON 출력 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-127">The JSON output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="fad4e-128">`appId`, `tenant` 및 `password` 값은 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-128">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="fad4e-129">`displayName`은(는) 기존 서비스 주체를 검색할 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-129">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="fad4e-130">계정에 서비스 주체를 만들기 위한 권한이 없는 경우, "권한이 부족하여 작업을 완료할 수 없습니다."가 포함된 오류 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-130">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="fad4e-131">서비스 주체를 만들려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="fad4e-131">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="fad4e-132">서비스 주체 역할 관리</span><span class="sxs-lookup"><span data-stu-id="fad4e-132">Manage service principal roles</span></span>

<span data-ttu-id="fad4e-133">Azure CLI는 역할 할당 관리를 위해 다음 명령을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-133">The Azure CLI provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="fad4e-134">az 역할 할당 나열</span><span class="sxs-lookup"><span data-stu-id="fad4e-134">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="fad4e-135">az 역할 할당 만들기</span><span class="sxs-lookup"><span data-stu-id="fad4e-135">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="fad4e-136">az 역할 할당 삭제</span><span class="sxs-lookup"><span data-stu-id="fad4e-136">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="fad4e-137">서비스 주체의 기본 역할은 **참가자**입니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-137">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="fad4e-138">이 역할은 Azure 계정에 대한 모든 읽기 및 쓰기 권한을 포함하며, 애플리케이션에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-138">This role has full permissions to read and write to an Azure account, and is not appropriate for applications.</span></span> <span data-ttu-id="fad4e-139">**Reader** 역할은 보다 제한적이며, 읽기 전용 액세스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-139">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="fad4e-140">RBAC(역할 기반 액세스 제어)와 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="fad4e-140">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="fad4e-141">이 예제에서는 **Reader** 역할을 추가하고 **Contributor** 역할을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-141">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="fad4e-142">역할을 추가해도 이전에 할당된 권한은 변경되지 _않습니다_.</span><span class="sxs-lookup"><span data-stu-id="fad4e-142">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="fad4e-143">서비스 주체 권한을 제한할 때는 항상 __Contributor__ 역할을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-143">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="fad4e-144">변경 사항은 할당된 역할을 나열하여 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-144">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="fad4e-145">계정에 역할 할당 권한이 없으면 계정에 "'/subscriptions/{guid}' 범위에 대해 'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 수 있는 권한이 없습니다." 오류 메시지가 표시됩니다. 역할을 관리하려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="fad4e-145">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="fad4e-146">서비스 주체를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="fad4e-146">Sign in using the service principal</span></span>

<span data-ttu-id="fad4e-147">Azure CLI 내에서 로그인하여 새로운 서비스 주체의 자격 증명 및 권한을 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-147">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="fad4e-148">`appId`, `tenant` 및 자격 증명 값을 사용하여 새로운 서비스 주체로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-148">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="fad4e-149">서비스 주체를 생성한 인증 유형을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-149">Use the authentication type that the service principal was created with.</span></span>

<span data-ttu-id="fad4e-150">암호를 사용하여 로그인하려면 암호를 인수 매개 변수로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-150">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="fad4e-151">인증서를 사용하여 로그인하려면 로컬 인증서를 PEM 또는 DER 파일로 사용할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-151">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="fad4e-152">자격 증명 다시 설정</span><span class="sxs-lookup"><span data-stu-id="fad4e-152">Reset credentials</span></span>

<span data-ttu-id="fad4e-153">서비스 주체의 자격 증명을 잊은 경우에는 [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) 명령으로 다시 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-153">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) command.</span></span> <span data-ttu-id="fad4e-154">여기에서도 새로운 서비스 주체를 만들 때와 동일한 제한 사항 및 옵션이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="fad4e-154">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID 
```

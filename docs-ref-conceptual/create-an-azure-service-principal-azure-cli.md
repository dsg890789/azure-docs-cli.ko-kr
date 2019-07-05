---
title: Azure CLI에서 Azure 서비스 주체 사용
description: Azure CLI를 사용하여 서비스 주체를 만들고 사용하는 방법을 알아봅니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6d88400b8d7070cf2f9dba2f3e124edfe2e3163d
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527331"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="eb29a-103">Azure CLI를 사용하여 Azure 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="eb29a-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="eb29a-104">Azure 서비스를 사용하도록 자동화된 도구에는 항상 제한된 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="eb29a-105">Azure는 애플리케이션에서 모든 권한이 있는 사용자로 로그인하도록 하는 대신 서비스 주체를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="eb29a-106">Azure 서비스 주체는 애플리케이션, 호스팅된 서비스 및 자동화된 도구에서 사용하여 Azure 리소스에 액세스하기 위해 만든 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="eb29a-107">이 액세스는 서비스 주체에 할당된 역할로 제한되므로 액세스할 수 있는 리소스와 해당 수준을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="eb29a-108">보안상의 이유로 사용자 ID를 통해 로그인할 수 있게 하는 대신, 항상 자동화된 도구에서 서비스 주체를 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="eb29a-109">이 문서에서는 Azure CLI를 사용하여 서비스 주체를 만들고, 정보를 가져오고, 다시 설정하는 단계를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="eb29a-110">서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="eb29a-110">Create a service principal</span></span>

<span data-ttu-id="eb29a-111">[az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) 명령을 사용하여 서비스 주체를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="eb29a-112">서비스 주체를 만드는 경우 사용하는 로그인 인증 유형을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span> 

> [!NOTE]
>
> <span data-ttu-id="eb29a-113">계정에 서비스 주체를 만들 수 있는 권한이 없는 경우 `az ad sp create-for-rbac`에서 "권한이 부족하여 작업을 완료할 수 없습니다."라는 오류 메시지를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="eb29a-114">서비스 주체를 만들려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="eb29a-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="eb29a-115">서비스 주체에 사용할 수 있는 인증 유형에는 암호 기반 인증 및 인증서 기반 인증의 두 가지 유형이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="eb29a-116">암호 기반 인증</span><span class="sxs-lookup"><span data-stu-id="eb29a-116">Password-based authentication</span></span>

<span data-ttu-id="eb29a-117">인증 매개 변수가 없으면 임의로 만든 암호를 통한 암호 기반 인증이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="eb29a-118">Azure CLI 2.0.68부터 약한 암호를 실수로 사용하는 것을 방지하기 위해 사용자 정의 암호로 서비스 주체를 만드는 `--password` 매개 변수가 __더 이상 지원되지 않습니다__.</span><span class="sxs-lookup"><span data-stu-id="eb29a-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="eb29a-119">암호 인증을 사용하는 서비스 주체의 출력에는 `password` 키가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="eb29a-120">이 값은 검색할 수 없으므로 __복사해야 합니다__.</span><span class="sxs-lookup"><span data-stu-id="eb29a-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="eb29a-121">암호를 잊어버린 경우 [서비스 주체 자격 증명을 다시 설정](#reset-credentials)하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="eb29a-122">`appId` 및 `tenant` 키는 `az ad sp create-for-rbac` 출력에 표시되며 서비스 주체 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="eb29a-123">해당 값은 기록하지만 언제든지 [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list)를 사용하여 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="eb29a-124">인증서 기반 인증</span><span class="sxs-lookup"><span data-stu-id="eb29a-124">Certificate-based authentication</span></span>

<span data-ttu-id="eb29a-125">인증서 기반 인증의 경우 `--cert` 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="eb29a-126">이 인수를 사용하려면 기존 인증서를 보유하고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="eb29a-127">이 서비스 주체를 사용하는 모든 도구에서 인증서의 프라이빗 키에 액세스할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="eb29a-128">인증서는 PEM, CER 또는 DER과 같은 ASCII 형식이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="eb29a-129">인증서를 문자열로 전달하거나 `@path` 형식을 사용하여 파일에서 인증서를 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="eb29a-130">Azure Key Vault에서 인증서를 사용하려면 `--keyvault` 인수를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-130">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="eb29a-131">이 경우 `--cert` 값은 인증서의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-131">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="eb29a-132">인증을 위해 _자체 서명된_ 인증서를 만들려면 `--create-cert` 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-132">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="eb29a-133">`--keyvault` 인수를 추가하면 Azure Key Vault에 인증서를 저장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-133">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="eb29a-134">`--keyvault`를 사용하는 경우 `--cert` 인수가 __필요합니다__.</span><span class="sxs-lookup"><span data-stu-id="eb29a-134">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="eb29a-135">인증서를 Key Vault에 저장하지 않으면 출력에 `fileWithCertAndPrivateKey` 키가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-135">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="eb29a-136">이 키의 값은 생성된 인증서가 저장되는 위치를 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-136">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="eb29a-137">인증서를 안전한 위치에 복사하거나 이 서비스 주체를 사용하여 로그인할 수 없는지 __확인해야 합니다__.</span><span class="sxs-lookup"><span data-stu-id="eb29a-137">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="eb29a-138">Key Vault에 저장된 인증서의 경우 [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show)를 사용하여 인증서의 프라이빗 키를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-138">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="eb29a-139">Key Vault에서 인증서의 비밀 이름은 인증서 이름과 동일합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-139">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="eb29a-140">인증서의 프라이빗 키에 액세스할 수 없는 경우 [서비스 주체 자격 증명](#reset-credentials)을 다시 설정하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-140">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="eb29a-141">`appId` 및 `tenant` 키는 `az ad sp create-for-rbac` 출력에 표시되며 서비스 주체 인증에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-141">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="eb29a-142">해당 값은 기록하지만 언제든지 [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list)를 사용하여 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-142">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="eb29a-143">기존 서비스 주체 가져오기</span><span class="sxs-lookup"><span data-stu-id="eb29a-143">Get an existing service principal</span></span>

<span data-ttu-id="eb29a-144">테넌트의 서비스 주체 목록은 [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list)를 사용하여 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-144">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="eb29a-145">이 명령은 기본적으로 테넌트에 대한 처음 100개의 서비스 주체를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-145">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="eb29a-146">테넌트의 서비스 주체를 모두 가져오려면 `--all` 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-146">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="eb29a-147">이 목록을 가져오는 데 시간이 오래 걸릴 수 있으므로 다음 인수 중 하나를 사용하여 목록을 필터링하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-147">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="eb29a-148">`--display-name`은 제공된 이름과 일치하는 _접두사_가 있는 서비스 주체를 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-148">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="eb29a-149">서비스 주체의 표시 이름은 만드는 중에 `--name` 매개 변수로 설정된 값입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-149">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="eb29a-150">서비스 주체 만드는 중에 `--name`을 설정하지 않은 경우 이름 접두사는 `azure-cli-`입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-150">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="eb29a-151">`--spn`은 정확한 서비스 주체 이름 일치 기준으로 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-151">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="eb29a-152">서비스 주체 이름은 항상 `https://`로 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-152">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="eb29a-153">`--name`에 사용한 값이 URI가 아닌 경우 이 값은 `https://`이며 바로 뒤에 표시 이름이 나옵니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-153">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="eb29a-154">`--show-mine`은 로그인한 사용자가 만든 서비스 주체만 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-154">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="eb29a-155">`--filter`는 OData 필터를 사용하며 _서버 쪽_ 필터링을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-155">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="eb29a-156">이 메서드는 CLI의 `--query` 인수를 사용하는 클라이언트 쪽 필터링보다 먼저 추천됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-156">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="eb29a-157">OData 필터에 대한 자세한 내용은 [필터에 대한 OData 식 구문](/rest/api/searchservice/odata-expression-syntax-for-azure-search)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-157">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="eb29a-158">서비스 주체 개체에 대해 반환되는 정보는 자세한 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-158">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="eb29a-159">로그인하는 데 필요한 정보만 가져오려면 `[].{"id":"appId", "tenant":"appOwnerTenantId"}` 쿼리 문자열을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-159">To get only the information necessary for sign-in, use the query string `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span></span> <span data-ttu-id="eb29a-160">예를 들어 현재 로그인한 사용자가 만든 모든 서비스 주체에 대한 로그인 정보를 가져오려면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-160">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query '[].{"id":"appId", "tenant":"appOwnerTenantId"}'
```

> [!IMPORTANT]
>
> <span data-ttu-id="eb29a-161">`az ad sp list` 또는 [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show)는 사용자와 테넌트를 가져오지만, 인증 비밀 _또는_ 인증 방법은 가져오지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-161">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="eb29a-162">Key Vault에 있는 인증서에 대한 비밀은 [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show)를 사용하여 검색할 수 있지만, 다른 비밀은 기본적으로 저장되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-162">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="eb29a-163">인증 방법 또는 비밀을 잊어버린 경우 [서비스 주체 자격 증명을 다시 설정](#reset-credentials)하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-163">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="eb29a-164">서비스 주체 역할 관리</span><span class="sxs-lookup"><span data-stu-id="eb29a-164">Manage service principal roles</span></span>

<span data-ttu-id="eb29a-165">역할 할당을 관리하기 위해 Azure CLI에는 다음과 같은 명령이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-165">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="eb29a-166">az 역할 할당 나열</span><span class="sxs-lookup"><span data-stu-id="eb29a-166">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="eb29a-167">az 역할 할당 만들기</span><span class="sxs-lookup"><span data-stu-id="eb29a-167">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="eb29a-168">az 역할 할당 삭제</span><span class="sxs-lookup"><span data-stu-id="eb29a-168">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="eb29a-169">서비스 주체의 기본 역할은 **참가자**입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-169">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="eb29a-170">이 역할에는 Azure 계정에서 읽고 쓸 수 있는 모든 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-170">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="eb29a-171">**Reader**(읽기 권한자) 역할은 읽기 전용 액세스 권한으로 더 제한적입니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-171">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="eb29a-172">RBAC(역할 기반 액세스 제어)와 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-172">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="eb29a-173">다음 예제에서는 **Reader** 역할을 추가하고 **Contributor**(기여자) 역할을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-173">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="eb29a-174">계정에 역할을 할당할 수 있는 권한이 없으면 계정에 "'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 수 있는 권한이 없습니다."라는 오류 메시지가 표시됩니다. 역할을 관리하려면 Azure Active Directory 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="eb29a-174">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="eb29a-175">역할을 추가해도 이전에 할당된 권한은 _제한되지 않습니다_.</span><span class="sxs-lookup"><span data-stu-id="eb29a-175">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="eb29a-176">서비스 주체 권한을 제한할 때는 __Contributor__ 역할을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-176">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="eb29a-177">변경 내용은 할당된 역할을 나열하여 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-177">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="eb29a-178">서비스 주체를 사용하여 로그인</span><span class="sxs-lookup"><span data-stu-id="eb29a-178">Sign in using a service principal</span></span>

<span data-ttu-id="eb29a-179">로그인하여 새 서비스 주체의 자격 증명과 권한을 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-179">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="eb29a-180">서비스 주체를 사용하여 로그인하려면 `appId`, `tenant` 및 자격 증명이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-180">To sign in with a service prinicpal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="eb29a-181">암호를 사용하는 서비스 주체로 로그인하려면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-181">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="eb29a-182">인증서를 사용하여 로그인하려면 해당 인증서를 ASCII 형식의 PEM 또는 DER 파일로 로컬로 사용할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-182">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="eb29a-183">서비스 주체를 사용하여 로그인하는 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="eb29a-183">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="eb29a-184">자격 증명 다시 설정</span><span class="sxs-lookup"><span data-stu-id="eb29a-184">Reset credentials</span></span>

<span data-ttu-id="eb29a-185">서비스 주체에 대한 자격 증명을 잊어버린 경우 [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset)을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-185">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="eb29a-186">reset 명령은 `az ad sp create-for-rbac`와 동일한 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="eb29a-186">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```

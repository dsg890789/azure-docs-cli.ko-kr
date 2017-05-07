---
title: "Azure CLI 2.0을 사용하여 Azure 서비스 주체 만들기"
description: "Azure CLI 2.0을 사용하여 앱 또는 서비스의 서비스 주체를 만드는 방법을 알아봅니다."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: 10a168ae0c33207905d58b7b57ac9ad76d8d9bf4
ms.sourcegitcommit: 73a73c8a17d95b116d33eee3287d938addc5c0ac
translationtype: HT
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Azure CLI 2.0을 사용하여 Azure 서비스 주체 만들기

Azure CLI 2.0을 사용하여 앱 또는 서비스를 관리하려는 경우 고유한 자격 증명 대신 AAD(Azure Active Directory) 서비스 주체에서 실행해야 합니다.
이 토픽에서는 Azure CLI 2.0을 사용하여 보안 주체를 만드는 과정을 설명합니다.

> [!NOTE]
> Azure Portal을 통해 서비스 주체를 만들 수도 있습니다.
> 자세한 내용은 [포털을 사용하여 리소스에 액세스할 수 있는 Active Directory 응용 프로그램 및 서비스 주체 만들기](/azure/azure-resource-manager/resource-group-create-service-principal-portal)를 참조하세요.

## <a name="what-is-a-service-principal"></a>'서비스 주체'란?

Azure 서비스 주체는 특정 Azure 리소스에 액세스하기 위해 사용자가 만든 앱, 서비스 및 자동화 도구에서 사용하는 보안 ID입니다. 특정한 역할이 있는 '사용자 ID'(로그인과 암호 또는 인증서)이며 리소스에 액세스하기 위해 엄격하게 제어됩니다. 일반 사용자 ID와 달리 특정 작업만을 수행해야 합니다. 해당 관리 작업을 수행하는 데 필요한 최소 사용 권한 수준을 부여하는 경우 보안이 향상됩니다. 

이제 Azure CLI 2.0은 암호 기반 인증 자격 증명 만들기만 지원합니다. 이 토픽에서는 특정 암호를 사용하여 서비스 주체를 만들고, 필요에 따라 서비스 주체에 특정 역할을 할당하는 방법을 다룹니다.

## <a name="verify-your-own-permission-level"></a>고유한 사용 권한 수준 확인

먼저 Azure Active Directory와 Azure 구독에 대한 충분한 권한이 있어야 합니다. 특히 Active Directory에서 앱을 만들고 서비스 주체에 역할을 할당할 수 있어야 합니다. 

계정에 적절한 사용 권한이 있는지를 확인하는 가장 쉬운 방법은 포털을 통하는 것입니다. [포털에서 필요한 사용 권한 확인](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions)을 참조하세요.

## <a name="create-a-service-principal-for-your-application"></a>응용 프로그램에 대한 서비스 주체 만들기

서비스 주체를 만들 앱을 식별하려면 다음 중 하나가 있어야 합니다.

  * 예제의 "MyDemoWebApp"처럼 배포된 앱의 고유한 이름 또는 URI
  * 응용 프로그램 ID, 배포된 앱/서비스/개체와 연결된 고유 GUID

이러한 값은 서비스 주체를 만들 때 응용 프로그램을 식별합니다.

### <a name="get-information-about-your-application"></a>응용 프로그램에 대한 정보 가져오기

`az ad app list`를 사용하여 응용 프로그램에 대한 ID 정보를 가져옵니다.

```azurecli
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

`--display-name` 옵션은 반환된 앱 목록을 필터링하여 `displayName`이 MyDemoWebApp으로 시작하는 앱만 표시합니다.

### <a name="create-the-service-principal"></a>서비스 주체 만들기

[az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac)를 사용하여 서비스 주체를 만듭니다. 

```azurecli
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
 > 안전하지 않은 암호를 만들지 마세요.  [Azure AD 암호 규칙 및 제한 사항](/azure/active-directory/active-directory-passwords-policy) 지침을 따르세요.

### <a name="get-information-about-the-service-principal"></a>서비스 주체에 대한 정보 가져오기

```azurecli
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

### <a name="sign-in-using-the-service-principal"></a>서비스 주체를 사용하여 로그인

이제 `az ad sp show`에서 *appId* 및 *암호*를 사용하여 앱의 새로운 서비스 주체로 로그인할 수 있습니다.  `az ad sp create-for-rbac` 결과에서 *테넌트* 값을 제공합니다.

```azurecli
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

성공적으로 로그온하면 이 출력이 표시될 것입니다.

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

앱을 실행하기 위한 자격 증명으로 `id`, `password` 및 `tenant` 값을 사용합니다. 

## <a name="managing-roles"></a>역할 관리 

> [!NOTE]
> Azure RBAC(역할 기반 액세스 제어)는 사용자 및 서비스 주체에 대한 역할을 정의하고 관리하기 위한 모델입니다.
> 역할에는 그와 관련된 일련의 사용 권한이 있으며 여기서 주체가 읽고 액세스하고 쓰고 관리할 수 있는 리소스를 결정합니다.
> RBAC와 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하세요.

Azure CLI 2.0은 역할 할당을 관리하는 다음 명령을 제공합니다.

* [az 역할 할당 나열](/cli/azure/role/assignment#list)
* [az 역할 할당 만들기](/cli/azure/role/assignment#create)
* [az 역할 할당 삭제](/cli/azure/role/assignment#delete)

서비스 주체의 기본 역할은 **참가자**입니다. 광범위한 사용 권한을 고려하면 앱과 Azure 서비스의 상호 작용을 위한 최상의 선택이 아닐 수도 있습니다. **판독기** 역할은 더 제한적이며 읽기 전용 액세스에 좋은 선택입니다. 역할 관련 사용 권한에 대한 세부 정보를 보거나 Azure Portal을 통해 사용자 지정 레코드를 만들 수 있습니다.

이 예제에서는 **판독기** 역할을 이전 예제에 추가하고 **참가자** 역할을 삭제합니다.

```azurecli
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

현재 할당된 역할을 나열하여 변경 내용을 확인합니다.

```azurecli
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
> 계정에 역할을 할당할 권한이 없는 경우 오류 메시지가 나타납니다.
> 이 메시지는 계정에 "/subscriptions/{guid}' 범위에 대해 'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 권한이 없다"는 내용입니다.
   
## <a name="change-the-credentials-of-a-security-principal"></a>보안 주체의 자격 증명 변경

사용 권한을 검토하고 암호를 정기적으로 업데이트하는 것은 좋은 보안 방법입니다. 앱이 변경되면 보안 자격 증명을 관리하고 수정할 수도 있습니다.

### <a name="reset-a-service-principal-password"></a>서비스 주체 암호 재설정

`az ad sp reset-credentials` 명령을 사용하여 서비스 주체의 현재 암호를 재설정할 수 있습니다.

```azurecli
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

`--password` 옵션을 생략하면 CLI가 안전한 암호를 생성합니다.
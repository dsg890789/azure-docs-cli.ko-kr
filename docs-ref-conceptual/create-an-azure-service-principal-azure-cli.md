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
# <a name="create-an-azure-service-principal-with-azure-cli"></a>Azure CLI를 사용하여 Azure 서비스 주체 만들기

액세스가 제한된 개별 로그인을 만들려면 서비스 주체를 통해 수행할 수 있습니다. 서비스 주체는 계정과 연결할 수 있는 별도의 ID입니다. 서비스 주체는 자동화해야 하는 애플리케이션 및 작업을 사용할 때 유용합니다. 이 문서에서는 서비스 주체를 만들기 위한 단계를 안내합니다.

## <a name="create-the-service-principal"></a>서비스 주체 만들기

[az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) 명령을 사용하여 서비스 주체를 만듭니다. 서비스 주체 이름은 기존 애플리케이션 또는 사용자 이름에 연결되지 않습니다. 원하는 인증 유형을 선택하여 서비스 주체를 만들 수 있습니다.

* `--password`은(는) 암호 기반 인증에 사용됩니다. 인증 형식을 나타내는 인수가 포함되지 않은 경우 기본적으로 암호가 사용되며 사용자를 위해 암호가 생성됩니다. 암호 기반 인증을 사용하려고 할 때 이 명령을 사용하도록 권장되며, 사용자를 위해 암호가 생성됩니다.  

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName 
  ```
  사용자를 위해 자동으로 생성되는 암호(보안상의 이유로 권장되지 않음) 대신 직접 암호를 설정하려고 할 때 이 명령을 사용하면 됩니다. [Azure Active Directory 암호 규칙 및 제한 사항](/azure/active-directory/active-directory-passwords-policy)에 따라 강력한 암호를 만들어야 합니다. 암호 설정 옵션에는 취약한 암호가 설정되거나 암호가 재사용될 가능성이 존재합니다. 이 옵션은 Azure CLI의 추후 버전에서는 사용되지 않을 계획입니다. 

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

* `--cert`은(는) 기존 인증서에 대한 인증서 기반 인증(PEM 또는 DER 공용 문자열) 또는 파일 로드를 위한 `@{file}`에 사용됩니다.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  인증서가 Azure Key Vault에 저장되는 것을 나타내기 위해서는 `--keyvault` 인수를 추가할 수 있습니다. 이 경우 `--cert` 값은 Key Vault에 있는 인증서 이름을 나타냅니다.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* `--create-cert`은(는) 인증을 위해 _자체 서명된_ 인증서를 만듭니다. `--cert` 인수가 제공되지 않으면 임의의 인증서 이름이 생성됩니다.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  `--keyvault` 인수를 추가하면 Azure Key Vault에 인증서를 저장할 수 있습니다. `--keyvault`을 사용하는 경우 `--cert` 인수 또한 필요합니다.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

인증 유형을 나타내는 인수가 포함되지 않은 경우, 기본적으로 `--password`이(가) 사용됩니다.

`create-for-rbac` 명령의 JSON 출력 형식은 다음과 같습니다.

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

`appId`, `tenant` 및 `password` 값은 인증에 사용됩니다. `displayName`은(는) 기존 서비스 주체를 검색할 때 사용됩니다.

> [!NOTE]
> 계정에 서비스 주체를 만들기 위한 권한이 없는 경우, "권한이 부족하여 작업을 완료할 수 없습니다."가 포함된 오류 메시지가 표시됩니다. 서비스 주체를 만들려면 Azure Active Directory 관리자에게 문의하십시오.

## <a name="manage-service-principal-roles"></a>서비스 주체 역할 관리

Azure CLI는 역할 할당 관리를 위해 다음 명령을 제공합니다.

* [az 역할 할당 나열](/cli/azure/role/assignment#az-role-assignment-list)
* [az 역할 할당 만들기](/cli/azure/role/assignment#az-role-assignment-create)
* [az 역할 할당 삭제](/cli/azure/role/assignment#az-role-assignment-delete)

서비스 주체의 기본 역할은 **참가자**입니다. 이 역할은 Azure 계정에 대한 모든 읽기 및 쓰기 권한을 포함하며, 애플리케이션에 적합하지 않습니다. **Reader** 역할은 보다 제한적이며, 읽기 전용 액세스를 제공합니다.  RBAC(역할 기반 액세스 제어)와 역할에 대한 자세한 내용은 [RBAC: 기본 제공 역할](/azure/active-directory/role-based-access-built-in-roles)을 참조하세요.

이 예제에서는 **Reader** 역할을 추가하고 **Contributor** 역할을 삭제합니다.

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

역할을 추가해도 이전에 할당된 권한은 변경되지 _않습니다_. 서비스 주체 권한을 제한할 때는 항상 __Contributor__ 역할을 제거해야 합니다.

변경 사항은 할당된 역할을 나열하여 확인할 수 있습니다.

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> 계정에 역할 할당 권한이 없으면 계정에 "'/subscriptions/{guid}' 범위에 대해 'Microsoft.Authorization/roleAssignments/write' 작업을 수행할 수 있는 권한이 없습니다." 오류 메시지가 표시됩니다. 역할을 관리하려면 Azure Active Directory 관리자에게 문의하십시오.

## <a name="sign-in-using-the-service-principal"></a>서비스 주체를 사용하여 로그인

Azure CLI 내에서 로그인하여 새로운 서비스 주체의 자격 증명 및 권한을 테스트할 수 있습니다. `appId`, `tenant` 및 자격 증명 값을 사용하여 새로운 서비스 주체로 로그인합니다. 서비스 주체를 생성한 인증 유형을 사용합니다.

암호를 사용하여 로그인하려면 암호를 인수 매개 변수로 제공합니다.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

인증서를 사용하여 로그인하려면 로컬 인증서를 PEM 또는 DER 파일로 사용할 수 있어야 합니다.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>자격 증명 다시 설정

서비스 주체의 자격 증명을 잊은 경우에는 [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) 명령으로 다시 설정할 수 있습니다. 여기에서도 새로운 서비스 주체를 만들 때와 동일한 제한 사항 및 옵션이 적용됩니다.

```azurecli-interactive
az ad sp credential reset --name APP_ID 
```

---
title: Azure CLI를 사용하여 Azure 구독 관리
description: Azure CLI를 사용하여 Azure 구독을 관리합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: f5fdfba785d849b1fd4f5919870ec9c341bb9c7d
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967812"
---
# <a name="manage-multiple-azure-subscriptions"></a>여러 Azure 구독 관리

대부분의 Azure 사용자는 단일 구독만 가집니다. 그러나, 사용자가 여러 조직에 속해 있거나 또는 여러 그룹에 걸친 특정 리소스에 액세스하기 위해 조직이 분할된 경우 Azure 내에서 여러 구독을 가질 수 있습니다. 모든 명령에 대한 전역 구독을 설정하거나 명령 기반으로 구독을 선택하여 CLI로 여러 구독을 쉽게 관리할 수 있습니다.

## <a name="tenants-users-and-subscriptions"></a>테넌트, 사용자 및 구독

Azure 내에서 테넌트, 사용자 및 구독 간의 차이에 대해 약간의 혼동이 있을 수 있습니다. _테넌트_는 전체 조직을 포괄하는 Azure Active Directory 엔터티입니다. 이 테넌트에는 하나 이상의 _구독_ 및 _사용자_가 있습니다. 사용자는 개인이며 소속된 조직인 테넌트 하나와만 연결됩니다. 사용자는 Azure에 로그인하여 리소스를 제공하고 사용하는 계정입니다.
사용자는 Azure를 포함하여 클라우드 서비스를 사용하기로 Microsoft와 계약한 여러 _구독_에 액세스할 수 있습니다. 모든 리소스가 구독과 연결됩니다.

테넌트, 사용자 및 구독 간의 차이점에 대한 자세한 내용은 [Azure 클라우드 용어 사전](/azure/azure-glossary-cloud-terminology)을 참조하세요.  새 구독을 Azure Active Directory 테넌트에 추가하는 방법을 알아보려면 [Azure 구독을 Azure Active Directory에 추가하는 방법](/azure/active-directory/active-directory-how-subscriptions-associated-directory)을 참조하세요.
여러 테넌트를 사용할 때 특정 테넌트에 로그인해야 합니다. 이 작업을 수행하려면 [Azure CLI 로그인](/cli/azure/authenticate-azure-cli)을 참조하세요.

## <a name="work-with-multiple-subscriptions"></a>여러 구독 작업

구독에 포함된 리소스에 액세스하려면 활성 구독을 전환해야 합니다. [az 계정 집합](/cli/azure/account#az-account-set)을 사용하거나 `--subscription` 인수를 사용하여 명령 기반으로 모든 Azure CLI 명령에 대해 구독을 전환할 수 있습니다.

시작하려면, 사용 가능한 구독 목록이 필요 합니다. 구독 목록을 가져오려면 [az 계정 목록](/cli/azure/account#az-account-list) 명령을 사용합니다:

```azurecli-interactive
az account list --output table
```

활성 구독을 전역으로 변경하려면 구독 ID 또는 구독 이름과 함께 `az account set`을 사용합니다:

```azurecli-interactive
az account set --subscription "My Demos"
```

명령에 대한 특정 구독을 사용하려면 `--subscription` 인수를 사용합니다. 이 인수는 구독 ID 또는 구독 이름을 사용합니다:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

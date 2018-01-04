---
title: "Azure CLI 2.0을 사용하여 여러 클라우드 관리"
description: "Azure CLI 2.0을 사용하여 여러 클라우드를 생성, 로그인 및 관리합니다."
keywords: "Azure CLI 2.0, Azure, 클라우드, 데이터 센터, 정부, 지역, 중국, 독일"
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 6f4cfec45becc0c4940e9066af53396b41db779d
ms.sourcegitcommit: 16426a08c0f2f62d0b9dca3df8132cece659acff
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/21/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Azure CLI 2.0을 사용하여 여러 클라우드 관리

서로 다른 영역에서 작업하거나 [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/)을 사용할 경우 하나 이상의 클라우드를 사용해야 할 수도 있습니다. Microsoft는 제품 사용에 적용될 수 있는 지역 법을 준수하기 위해 클라우드를 제공합니다. 이 문서에서는 계정에서 사용할 수 있는 클라우드에 대한 정보를 얻고 현재 클라우드를 변경하고 Azure Stack에서 사용할 새 클라우드를 등록 또는 등록 취소하는 방법을 설명합니다.

## <a name="listing-clouds"></a>클라우드 나열

[cloud list](/cli/azure/cloud#list) 명령을 사용하여 사용 가능한 클라우드를 나열할 수 있습니다. 이렇게 하면 현재 활성 클라우드, 현재 프로필, 지역별 접미사 및 호스트 이름에 대한 정보를 알 수 있습니다.

활성 클라우드와 모든 사용 가능한 클라우드 목록을 가져오려면:

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

현재 활성 클라우드에는 `IsActive` 열에 `True`가 있습니다. 언제든지 하나의 클라우드만 활성화할 수 있습니다. Azure 서비스에 사용하는 끝점을 포함하여 클라우드에 대한 자세한 정보를 알아보려면 `cloud show` 명령을 사용하세요.

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a>활성 클라우드 전환

현재 활성 클라우드를 전환하려면 [cloud set](/cli/azure/cloud#set) 명령을 실행합니다. 이 명령은 하나의 필수 인수인 클라우드 이름을 사용합니다.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> 활성화된 클라우드에 대한 인증이 만료된 경우에 다른 CLI 작업을 수행하기 전에 다시 인증해야 합니다. 새로운 클라우드로 처음 전환하는 경우도 활성 구독을 설정해야 합니다.
> 인증에 대한 지침은 [Azure CLI 2.0을 사용하여 로그인](authenticate-azure-cli.md)을 참조하세요. 구독 관리에 대한 자세한 내용은 [Azure CLI 2.0을 사용하여 Azure 구독 관리](manage-azure-subscriptions-azure-cli.md)를 참조하세요.

## <a name="register-a-cloud"></a>클라우드 등록

Azure Stack에 대한 사용자 고유의 끝점이 있는 경우 새 클라우드를 등록합니다. 클라우드를 만들려면 [cloud register](/cli/azure/cloud#register) 명령을 사용합니다. 이 명령에는 이름 그리고 연관된 끝점이 있는 기능 집합이 필요합니다. Azure Stack과 함께 사용할 클라우드를 등록하는 방법에 대해 알아보려면 [Azure Stack과 함께 사용할 CLI 설치 및 구성](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack)을 참조하세요.

중국, 미국 정부 또는 독일 지역의 경우 클라우드를 등록할 필요가 없습니다. 이들 지역은 Microsoft에서 관리하며 기본적으로 사용할 수 있습니다.  사용 가능한 모든 끝점 설정에 대한 자세한 내용은 에 대한 [ 설명서를 참조하세요 `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).

클라우드를 등록하더라도 자동으로 해당 클라우드로 전환되지 않습니다. 위에서 설명한 대로 `az cloud set` 명령을 사용하여 새로 만든 클라우드를 선택합니다.

## <a name="update-an-existing-cloud"></a>기존 클라우드 업데이트

권한이 있는 경우 기존 클라우드를 업데이트할 수도 있습니다. 다른 Azure 프로필로 전환하거나 끝점을 추가하거나 끝점을 변경해야 하는 경우 이를 수행합니다.
`az cloud register`과 동일한 인수를 사용하여 `az cloud update` 명령으로 이 작업을 수행합니다. 자세한 내용은 의 [ 설명서를 참조하세요`az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).

## <a name="unregister-a-cloud"></a>클라우드 등록 취소

등록한 클라우드가 더 이상 필요하지 않으면 [cloud unregister](/cli/azure/cloud#unregister) 명령을 사용하여 등록을 취소할 수 있습니다.

```azurecli
az cloud unregister --name MyCloud
```

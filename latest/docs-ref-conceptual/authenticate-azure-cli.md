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
ms.openlocfilehash: 3ba1dd840102c738ccd9eb62a0b9db612cec48d1
ms.sourcegitcommit: 5cfbea569fef193044da712708bc6957d3fb557c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/14/2017
---
# <a name="log-in-with-azure-cli-20"></a>Azure CLI 2.0으로 로그인

Azure CLI를 사용하여 로그인하고 인증하는 여러 방법이 있습니다. 가장 간단하게 시작하는 방법은 브라우저를 통해 대화형으로 로그인하거나 명령줄에서 로그인하는 것입니다. 리소스를 조작하는 데 사용할 수 있는 비 대화형 계정을 만드는 방법을 제공하는 서비스 주체를 사용할 것을 권장합니다. 서비스 주체에게 필요한 접근 권한만 부여하여 자동화 스크립트를 훨씬 안전하게 보호할 수 있습니다. 

개인 자격 증명 정보는 로컬로 저장되지 않습니다. 대신, Azure에서 인증 토큰이 생성되고 저장됩니다. 로그인한 후에 사용하지 않고 14일이 지날 때까지 사용자 로컬 로그인 토큰이 유효합니다. 이 시점에 다시 인증해야 합니다.

CLI를 사용하여 실행하는 명령은 기본 구독에 대해 실행됩니다.  둘 이상의 구독이 있는 경우 [기본 구독을 확인](manage-azure-subscriptions-azure-cli.md)하고 적절하게 변경합니다.

## <a name="interactive-log-in"></a>대화형 로그인

웹 브라우저에서 대화형으로 로그인합니다.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>명령 줄

명령줄에 자격 증명을 입력합니다.

> [!Note]
> 이 접근 방식은 Microsoft 계정 또는 2단계 인증을 사용하는 계정에서는 작동하지 않습니다.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>서비스 주체로 로그인

서비스 주체는 Azure Active Directory를 사용하여 규칙을 적용할 수 있는 사용자 계정과 비슷합니다.
리소스를 조작하는 스크립트 또는 응용 프로그램에서 Azure 리소스 사용을 보호하는 가장 좋은 방법은 서비스 주체를 사용하여 인증하는 것입니다.
`az role` 명령 집합을 통해 사용자에게 줄 역할을 정의합니다.
[az 역할 참조 문서](https://docs.microsoft.com/cli/azure/role.md)에서 서비스 주체 역할의 자세한 내용과 예제를 살펴볼 수 있습니다.

1. 아직 서비스 주체가 없는 경우 [하나 만듭니다](create-an-azure-service-principal-azure-cli.md).

1. 서비스 주체로 로그인합니다.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   테넌트를 가져오려면 대화형으로 로그인한 다음 구독에서 tenantId를 가져옵니다.

   ```azurecli
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

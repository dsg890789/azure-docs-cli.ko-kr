---
title: Azure CLI 2.0으로 로그인
description: Azure CLI 2.0을 사용하여 대화형으로 또는 로컬 자격 증명을 사용하여 로그인
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/13/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: bbd64458b49d3e6c6a533a489d5c8105f364d3d7
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439876"
---
# <a name="log-in-with-azure-cli-20"></a>Azure CLI 2.0으로 로그인

Azure CLI를 사용하여 로그인하고 인증하는 여러 방법이 있습니다. 가장 간단하게 시작하는 방법은 Azure Cloud Shell을 통해 브라우저에서 대화형으로 또는 `az login` 명령으로 로그인하는 것입니다.
권장되는 접근 방법은 권한 제한 계정인 서비스 주체를 사용하는 것입니다. 서비스 주체에게 필요한 접근 권한만 부여하여 자동화 스크립트를 훨씬 안전하게 보호할 수 있습니다.

개인 자격 증명 정보는 로컬로 저장되지 않습니다. 대신, Azure에서 인증 토큰이 생성되고 저장됩니다. 로그인 후에는 사용되지 않더라도 로그인 토큰이 14일 동안 유효합니다. 그 다음에는 다시 인증해야 합니다.

로그인한 후 CLI 명령은 기본 구독에 대해 실행됩니다. 구독이 두 개 이상인 경우 [기본 구독 변경](manage-azure-subscriptions-azure-cli.md)을 수행할 수 있습니다.

## <a name="interactive-sign-in"></a>대화형 로그인

Azure CLI의 기본 인증 방법은 웹 브라우저에서 대화형으로 로그인하는 것입니다.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>명령 줄

명령줄에 Azure 사용자 자격 증명을 입력합니다.

> [!Note]
> 이 접근 방식은 Microsoft 계정 또는 2단계 인증을 사용하는 계정에서는 작동하지 않습니다.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> 콘솔에 암호를 표시하지 않고 `az login`을 대화식으로 사용하려는 경우 `bash`에서 `read -s` 명령을 사용합니다.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> PowerShell에서 `Read-Host -AsSecureString` cmdlet를 사용하고 문자열 변환을 보호합니다.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="log-in-with-a-specific-tenant"></a>특정 테넌트로 로그인

여러 테넌트를 사용할 때 `--tenant` 인수를 사용하여 로그인할 테넌트를 선택할 수 있습니다. 이 인수의 값은 `.onmicrosoft.com` 도메인 또는 테넌트에 대한 Azure 개체 ID일 수 있습니다. 대화형으로 로그인하거나 `--user` 및 `--password` 인수를 포함한 자격 증명을 제공할 수 있습니다. 

```azurecli
az login --tenant <tenant>
```

## <a name="log-in-with-a-service-principal"></a>서비스 주체를 사용하여 로그인

서비스 주체는 특정 사용자에게 연결되지 않은 계정으로서, 미리 정의된 역할을 통해 사용자에게 권한을 할당할 수 있습니다. 보안 스크립트 또는 프로그램 작성을 위한 가장 좋은 방법은 권한 제한 사항 및 로컬로 저장된 정적 자격 증명 정보를 적용할 수 있게 해주는 서비스 주체를 사용한 인증입니다. 서비스 주체에 대해 자세히 알아보려면 [Azure CLI를 사용하여 Azure 서비스 주체 만들기](create-an-azure-service-principal-azure-cli.md)를 참조하십시오.

서비스 주체로 로그인하려면 사용자 이름, 암호 또는 인증서 PEM 파일 및 서비스 주체와 연결된 테넌트를 제공합니다.

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

테넌트 값은 서비스 주체와 연결된 Azure Active Directory 테넌트입니다. 이 값은 `.onmicrosoft.com` 도메인 또는 테넌트에 대한 Azure 개체 ID일 수 있습니다.
다음 명령을 사용하여 현재 로그인을 위한 테넌트 개체 ID를 가져올 수 있습니다.

```azurecli-interactive
az account show --query 'tenantId' -o tsv
```

> [!IMPORTANT]
> 콘솔에 암호를 표시하지 않고 `az login`을 대화식으로 사용하려는 경우 `bash`에서 `read -s` 명령을 사용합니다.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> PowerShell에서 `Read-Host -AsSecureString` cmdlet를 사용하고 문자열 변환을 보호합니다.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```

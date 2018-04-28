---
title: Azure CLI 구성 옵션
description: Azure CLI 2.0 구성 방법
keywords: Azure CLI, 구성, 설정, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/13/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: be5938dcee360932342b4867728516e8ddd4a7cf
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2018
---
# <a name="azure-cli-20-configuration"></a>Azure CLI 2.0 구성

Azure CLI 2.0을 사용하면 사용자 구성에서 로깅 및 데이터 수집과 같은 내부 설정을 무시하고 일부 필수 매개 변수에 대한 기본 옵션을 제공할 수 있습니다. CLI는 이러한 값 중 일부인 `az configure`를 관리하기 위한 편리한 명령을 제공하며, 다른 값은 구성 파일에서 또는 환경 변수를 사용하여 설정할 수 있습니다.

CLI에서 사용되는 구성 값은 다음 우선 순위에서 평가되며 목록의 상위 항목이 우선 순위를 갖습니다.

1. 명령줄 매개 변수
2. 환경 변수
3. 구성 파일의 값 또는 `az configure`로 사용

## <a name="cli-configuration-with-az-configure"></a>az configure으로 CLI 구성

[az configure](/cli/azure/reference-index#az-configure) 명령으로 CLI에 대한 기본값을 설정합니다.
이 명령은 하나의 인수인 `--defaults`를 취하며 공백으로 구분된 `key=value` 쌍의 목록입니다. 제공된 값은 필수 인수 대신 CLI에 의해 사용됩니다.

다음은 사용할 수 있는 사용 가능한 키 목록입니다.

| Name | 설명 |
|------|-------------|
| group | 모든 명령에 사용할 기본 리소스 그룹입니다. |
| location | 모든 명령에 사용할 기본 위치입니다. |
| web | `az webapp` 명령에 사용할 기본 앱입니다. |
| vm | `az vm` 명령에 사용할 기본 VM 이름입니다. |
| vmss | `az vmss` 명령에 사용할 기본 VMSS 이름입니다. |
| acr | `az acr` 명령에 사용할 기본 컨테이너 레지스트리 이름입니다. |
| acs | `az acs` 명령에 사용할 기본 컨테이너 서비스 이름입니다. |

예를 들어, 다음은 모든 명령에 대해 기본 리소스 그룹 및 위치를 설정하는 방법입니다.

```azurecli
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>CLI 구성 파일

CLI 구성 파일에는 CLI 동작 관리에 사용되는 다른 설정이 포함됩니다. 구성 파일 자체는 `$AZURE_CONFIG_DIR/config`에 있습니다. `AZURE_CONFIG_DIR`의 기본값은 Linux와 macOS의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다.

구성 파일은 INI 파일 형식으로 작성됩니다. 이 파일들은 `[section-name]` 헤더로 시작하고 그 다음 `key=value` 항목 목록이 이어지는 섹션으로 구성됩니다. 세션 이름은 대/소문자를 구분하지만, 키 이름은 구분하지 않습니다.
설명은 `#` 또는 `;`으로 시작하는 줄입니다. 인라인 주석은 허용되지 않습니다. 부울은 대/소문자를 구분하며 다음 값으로 표현됩니다.

* __True__: 1, 예, true, on
* __False__: 0, 아니요, false, off

다음은 확인 프롬프트를 비활성화하고 `/var/log/azure` 디렉토리에 로깅을 설정하는 CLI 구성 파일의 예입니다.

```
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

모든 사용 가능한 구성 값과 그 의미에 대한 자세한 내용은 다음 섹션을 참조하세요. INI 파일 형식에 전체 세부 정보는 [INI에 대한 Python 문서](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure)를 참조하세요.

## <a name="cli-configuration-values-and-environment-variables"></a>CLI 구성 값 및 환경 변수

다음 표에는 구성 파일에 배치할 수 있는 모든 섹션 및 옵션 이름이 포함되어 있습니다. 해당 환경 변수는 모두 대문자로 `AZURE_{section}_{name}`로서 설정할 수 있습니다. 예를 들어, `AZURE_BATCHAI_STORAGE_ACCOUNT` 변수에서 `batchai` 섹션의 `storage_account` 기본값을 설정할 수 있습니다.

사용할 수 있는 기본값의 값은 필요한 경우 명령줄 인수에 있지 않아도 됩니다.

| 섹션 | Name      | type | 설명|
|---------|-----------|------|------------|
| __core__ | output | string | 기본 출력 형식입니다. `json`, `jsonc`, `tsv` 또는 `table` 중 하나일 수 있습니다. |
| | disable\_confirm\_prompt | 부울 | 확인 메시지를 표시하거나 표시하지 않습니다. |
| | collect\_telemetry | 부울 | Microsoft가 CLI의 사용에 대해 익명의 데이터를 수집하도록 허용합니다. 개인 정보에 대한 자세한 내용은 [Azure CLI 2.0 사용 약관](http://aka.ms/AzureCliLegal)을 참조하세요. |
| __logging__ | enable\_log\_file | 부울 | 로깅을 켜거나 끕니다. |
| | log\_dir | string | 로그를 쓸 디렉터리입니다. 기본적으로 `${AZURE_CONFIG_DIR}/logs`입니다. |
| __storage__ | connection\_string | string | `az storage` 명령에 사용할 기본 연결 문자열입니다. |
| | 계정 | string | `az storage` 명령에 사용할 기본 계정 이름입니다. |
| | key | string | `az storage` 명령에 사용할 기본 계정 키입니다. |
| | sas\_token | string | `az storage` 명령에 사용할 기본 SAS 토큰입니다. |
| __batchai__ | storage\_account | string | `az batchai` 명령에 사용할 기본 저장소 계정입니다. |
| | storage\_key | string | `az batchai` 명령에 사용할 기본 저장소 키입니다. |
| __batch__ | 계정 | string | `az batch` 명령에 사용할 기본 Azure Batch 계정 이름입니다. |
| | access\_key | string | `az batch` 명령에 사용할 기본 액세스 키입니다. `aad` 권한 부여와 함께 사용됩니다. |
| | endpoint | string | `az batch` 명령에 대해 연결할 기본 끝점입니다. |
| | auth\_mode | string | `az batch` 명령에 사용할 권한 부여 모드입니다. `shared_key` 또는 `aad`일 수 있습니다. |

> [!NOTE]
> 구성 파일에 다른 값이 표시될 수 있지만 이는 `az configure`를 포함하여 CLI 명령을 통해 직접 관리됩니다. 위의 표에 나열된 것은 사용자가 직접 변경해야 하는 값입니다.

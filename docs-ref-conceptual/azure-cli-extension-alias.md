---
title: Azure CLI 2.0 별칭 확장
description: Azure CLI 2.0 별칭 확장 사용 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e457d78b1009fe573554df36db18f525516e0b4a
ms.sourcegitcommit: 335c11e6c34f7907e61a43507745ba84ed4e7469
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2018
---
# <a name="the-azure-cli-20-alias-extension"></a>Azure CLI 2.0 별칭 확장

별칭 확장을 사용하면 기존 명령을 사용하여 Azure CLI에 대한 사용자 정의 명령을 정의할 수 있습니다. 별칭을 사용하면 바로 가기를 허용하고 위치 인수를 사용할 수 있으므로 워크플로를 간결하고 간단하게 유지할 수 있습니다. 별칭은 Jinja2 템플릿 엔진을 기반으로 하기 때문에 고급 인수 처리도 제공합니다.

> [!NOTE]
> 별칭 확장은 공개 미리 보기에 있습니다. 기능 및 구성 파일 형식이 변경될 수 있습니다.

## <a name="install-the-alias-extension"></a>별칭 확장 설치

별칭 확장을 사용하는 데 필요한 최소 Azure CLI 버전은 **2.0.28**입니다. CLI 버전을 확인하려면 `az --version`을 실행합니다. 설치를 업데이트해야 하는 경우 [Azure CLI 2.0 설치](./install-azure-cli.md)의 지침을 따릅니다.

[az extension add](/cli/azure/extension#az-extension-add) 명령을 사용하여 확장을 설치합니다.

```azurecli
az extension add --name alias
```

[az 확장 목록](/cli/azure/extension#az-extension-list)을 사용하여 확장 설치를 확인합니다. 별칭 확장이 제대로 설치된 경우 명령 출력에 나열됩니다.

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a>확장을 최신 상태로 유지

별칭 확장은 현재 개발 중이며 새 버전은 정기적으로 릴리스됩니다. 새 버전은 CLI를 업데이트할 때마다 자동으로 설치되지 않습니다. [az 확장 업데이트](/cli/azure/extension#az-extension-update)를 사용하여 확장 업데이트를 설치합니다.

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a>별칭 명령 파일 형식

별칭 명령 정의는 `$AZURE_USER_CONFIG/alias`에있는 구성 파일에 작성됩니다. `AZURE_USER_CONFIG`의 기본값은 macOS와 Linux의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다. 별칭 구성 파일은 INI 구성 파일 형식으로 작성됩니다. 별칭 명령의 일반적인 형식은 다음과 같습니다.

```
[command_name]
command = invoked_commands
```

명령의 일부로 `az`를 포함하지 마세요.

## <a name="create-simple-alias-commands"></a>간단한 별칭 명령 만들기

별칭을 사용하면 기존 명령 그룹이나 명령 이름을 단축할 수 있습니다. 예를 들어 `group` 명령 그룹을 `rg`로, `list` 명령을 `ls`로 단축할 수 있습니다.

```
[rg]
command = group

[ls]
command = list
```

이렇게 새로 정의된 별칭은 정의가 될 수 있는 어느 곳에서든 사용할 수 있습니다.

```azurecli
az rg list
az rg ls
az vm ls
```

별칭은 전체 명령의 바로 가기일 수도 있습니다. 다음 예는 사용 가능한 리소스 그룹과 해당 위치를 테이블로 출력하여 나열합니다.

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

이제 `ls-groups`는 다른 CLI 명령처럼 실행될 수 있습니다.

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a>인수를 사용하여 별칭 명령 만들기

별칭 이름에 위치 인수를 `{{ arg_name }}`으로 포함하여 별칭 명령에 추가할 수도 있습니다. 중괄호 안의 공백이 필요 합니다.

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

다음 예제 별칭은 위치 인수를 사용하여 VM의 공용 IP 주소를 얻는 방법을 보여줍니다.

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

이 명령을 실행할 때 위치 인수에 값을 제공합니다.

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

별칭으로 호출된 명령에서 환경 변수를 사용할 수도 있으며, 이 명령은 런타임에서 평가됩니다. 다음 예는 `eastus`에 리소스 그룹을 만들고 `owner` 태그를 추가하는 `create-rg` 별칭을 추가합니다. 이 태그에는 로컬 환경 변수 `USER`의 값이 지정됩니다.

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a>Jinja2 템플릿을 사용하는 프로세스 인수

별칭 확장의 인수 대체는 [Jinja2](http://jinja.pocoo.org/docs/2.10/)에 의해 수행되어 Jinja2 템플릿 엔진의 기능에 대한 모든 액세스 권한을 제공합니다. 템플릿을 사용하면 문자열에서 데이터 추출 및 대체와 같은 작업을 수행할 수 있습니다.

Jinja2 템플릿을 사용하면 기본 명령과 다른 인수 유형을 사용하는 별칭을 작성할 수 있습니다. 예를 들어 저장소 URL을 사용하는 별칭을 만들 수 있습니다. 그런 다음 이 URL을 구문 분석하여 계정 및 컨테이너 이름을 저장소 명령에 전달합니다.

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

Jinja2 템플릿 엔진에 대한 자세한 내용은 [Jinja2 설명서](http://jinja.pocoo.org/docs/2.10/templates/)를 참조하세요.

## <a name="uninstall-the-alias-extension"></a>별칭 확장 제거

확장을 설치 제거하려면 [az extension remove](/cli/azure/extension#az-extension-remove) 명령을 사용합니다.

```azurecli
az extension remove --name alias
```

확장 관련 버그 또는 기타 문제로 인해 제거한 경우 [GitHub 문제를 제출](https://github.com/Azure/azure-cli-extensions/issues)하면 수정 사항을 받을 수 있습니다.

---
title: Azure CLI 2.0 확장
description: Azure CLI 2.0 확장 사용
keywords: Azure CLI, 확장
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b503c51ffc55ceda30738e34171c7da92532f328
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967727"
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Azure CLI 2.0 확장 사용

확장은 Azure CLI 자체와 함께 제공되지 않는 새로운 명령을 통해 기능을 추가하는 개별 모듈입니다. 이러한 확장은 Microsoft에서 제공하는 전문 도구 또는 사용자가 직접 작성하는 사용자 지정 기능과 같은 실험적인 기능 또는 릴리스 전 기능으로 제공될 수 있습니다. 확장을 사용하면 CLI를 통해 유연성을 갖출 수 있으므로 핵심 기능 집합의 일부로 간주되지 않는 많은 추가 패키지를 제공하지 않고도 자신의 요구 사항에 맞게 수정할 수 있습니다.

이 문서에서는 CLI에 대한 확장을 설치, 업데이트 및 제거하는 방법을 설명합니다. 또한 확장 동작에 대한 일반적인 질문에 답변합니다.

## <a name="find-extensions"></a>확장 찾기

[az extension list-available](/cli/azure/extension#az-extension-list-available)을 사용하면 사용할 수 있는 확장을 확인할 수 있습니다. 이 명령은 Microsoft에서 제공하고 관리하는 공식 확장 프로그램을 나열합니다.

```azurecli-interactive
az extension list-available --output table
```

설명서 사이트에도 [ Microsoft 확장 목록 ](azure-cli-extensions-list.md)이 있습니다.

## <a name="install-extensions"></a>확장 설치

설치할 확장을 찾은 다음에는 [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add)를 사용하여 가져옵니다. 확장이 `az extension list-available`에 나열된 경우 해당 이름으로 확장을 설치할 수 있습니다.

```azurecli-interactive
az extension add --name <extension-name>
```

확장이 외부 리소스에 있거나 직접 연결되는 링크가 있는 경우 원본 URL 또는 로컬 경로를 제공할 수 있습니다. 이는 _컴파일된 Python 휠 파일이어야 합니다_.

```azurecli-interactive
az extension add --source <URL-or-path>
```

확장이 설치되었으면 `$AZURE_EXTENSION_DIR` 셸 변수 값에서 이 파일을 찾을 수 있습니다. 이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.

## <a name="update-extensions"></a>확장 업데이트

확장이 이름별로 설치된 경우 [az 확장 업데이트](https://docs.microsoft.com/cli/azure/extension#az-extension-update)를 사용하여 업데이트할 수 있습니다.

```azurecli-interactive
az extension update --name <extension-name>
```

그렇지 않으면 [설치 확장](#install-extensions) 지침에 따라 소스에서 확장을 업데이트할 수 있습니다.

CLI가 확장 이름을 해석할 수 없는 경우 이를 제거하고 다시 설치합니다. 확장이 미리 보기에서 CLI의 기본 명령으로 전환되었을 수도 있습니다. [Azure CLI 2.0 설치](install-azure-cli.md)에 설명된 대로 CLI를 업데이트하고 확장 프로그램의 명령이 추가되었는지 확인합니다.

## <a name="uninstall-extensions"></a>확장 제거

확장이 더 이상 필요하지 않으면 [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove)를 사용하여 제거할 수 있습니다.

```azurecli-interactive
az extension remove --name <extension-name>
```

확장을 설치한 위치에서 수동으로 삭제하여 제거할 수도 있습니다. 이는 `$AZURE_EXTENSION_DIR` 셸 변수의 값입니다.
이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

`az extension remove`를 사용하여 제거하는 것이 좋습니다.

## <a name="faq"></a>FAQ

다음은 CLI 확장에 대한 몇 가지 다른 일반적인 질문에 대한 답변입니다.

### <a name="what-file-formats-are-allowed-for-installation"></a>설치에 사용할 수 있는 파일 형식은 무엇인가요?

현재 컴파일된 Python 휠 파일만 확장으로 설치할 수 있습니다.

### <a name="can-extensions-replace-existing-commands"></a>확장에서 기존 명령을 바꿀 수 있나요?

예. 확장에서 기존 명령을 바꿀 수 있지만, 바꾼 명령이 실행되기 전에 CLI에서 경고가 발생합니다.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>확장이 시험판인지 어떻게 알 수 있나요?

확장이 시험판인 경우 자체 설명서 및 버전 관리를 통해 표시됩니다. 또한 Microsoft에서 일반적으로 제품을 미리 보기에서 기본 CLI 인터페이스로 전환하는 계획을 통해 CLI에 대한 미리 보기 명령을 확장으로 제공합니다.

### <a name="can-extensions-depend-upon-each-other"></a>확장은 서로 종속될 수 있나요?

아니요. 확장은 각각 독립적인 개별 패키지입니다. 이는 CLI에서 확장이 로드되는 시기를 보장하지 않으므로 종속성이 충족되지 못할 수 있기 때문입니다. 확장을 설치하는 경우 해당 확장만 설치되며 다른 확장을 제거하더라도 계속 작동합니다.

### <a name="are-extensions-updated-along-with-the-cli"></a>확장은 CLI와 함께 업데이트되나요?

아니요. [확장 업데이트](#update-extensions)에 설명된 대로 확장은 별도로 업데이트해야 합니다.

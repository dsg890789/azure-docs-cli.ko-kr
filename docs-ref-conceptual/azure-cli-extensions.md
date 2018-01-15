---
title: "Azure CLI 2.0 확장"
description: "Azure CLI 2.0 확장 사용"
keywords: "Azure CLI, 확장"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a76e58c4430a184d133cca0ef0623f325aeb2f27
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Azure CLI 2.0 확장 사용

확장은 새 명령을 통해 기능을 추가할 수 있는 Azure CLI 자체와 함께 제공되지 않는 개별 모듈입니다. 이러한 모듈은 실험적 또는 시험판 제품, Microsoft에서 사용자의 요구에 맞춘 특수 도구 또는 사용자가 직접 작성한 확장일 수 있습니다. 확장을 사용하면 CLI를 통해 유연성을 갖출 수 있으므로 핵심 기능 집합의 일부로 간주되지 않는 많은 추가 패키지를 제공하지 않고도 자신의 요구 사항에 맞게 수정할 수 있습니다.

이 문서는 CLI 확장을 설치, 업데이트 및 제거하는 방법을 이해하는 데 도움이 됩니다. 또한 확장 동작에 대한 일반적인 질문에 대답하고 있습니다.

## <a name="finding-extensions"></a>확장 찾기

`az extension list-available`을 사용하면 사용 가능한 확장을 확인할 수 있습니다. 이 명령은 Microsoft에서 제공하고 지원하는 사용 가능한 공식 확장을 나열합니다.

## <a name="installing-extensions"></a>확장 설치

설치할 확장을 찾았으면 `az extension add`을 사용하여 가져옵니다. 확장이 `az extension list-available`에 나열된 공식 Microsoft 확장인 경우 확장을 이름별로 설치할 수 있습니다.

```azurecli
az extension add --name <extension-name>
```

확장이 외부 리소스에 있거나 직접 연결되는 링크가 있는 경우 원본 URL 또는 로컬 경로를 제공할 수 있습니다. 이는 _컴파일된 Python 휠 파일이어야 합니다_.

```azurecli
az extension add --source <URL-or-path>
```

확장이 설치되었으면 `$AZURE_EXTENSION_DIR` 셸 변수 값에서 이 파일을 찾을 수 있습니다. 이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.

## <a name="updating-extensions"></a>확장 업데이트

확장은 이름별로만 업데이트할 수 있습니다.

```azurecli
az extension update --name <extension-name>
```

어떤 이유로든 CLI에서 확장 이름을 확인할 수 없으면 확장을 다시 설치하여 업데이트합니다. 확장이 미리 보기에서 CLI의 기본 명령으로 전환되었을 수도 있습니다. 이 경우 CLI를 업데이트하고 확장을 제거합니다.

## <a name="uninstalling-extensions"></a>확장 제거

확장이 더 이상 필요하지 않으면 `az extension remove`를 사용하여 제거할 수 있습니다.

```azurecli
az extension remove --name <extension-name>
```

확장을 설치한 위치에서 수동으로 삭제하여 제거할 수도 있습니다. 이는 `$AZURE_EXTENSION_DIR` 셸 변수의 값입니다. 이 변수가 설정되어 있지 않으면 기본적으로 Linux 및 macOS에서는 `$HOME/.azure/cliextensions`, Windows에서는 `%USERPROFILE%\.azure\cliextensions`입니다.

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

번호 확장은 각각 독립적인 개별 패키지입니다. 이는 CLI에서 확장이 로드되는 시기를 보장하지 않으므로 종속성이 충족되지 못할 수 있기 때문입니다. 확장을 설치하는 경우 해당 확장만 설치되며 다른 확장을 제거하더라도 계속 작동합니다.

### <a name="are-extensions-updated-along-with-the-cli"></a>확장은 CLI와 함께 업데이트되나요?

번호 [확장 업데이트](#updating-extensions) 섹션에서 설명한 대로 확장은 별도로 업데이트해야 합니다.

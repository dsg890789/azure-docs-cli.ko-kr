---
title: "macOS용 Azure CLI 설치"
description: "macOS에 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure macos, azure 설치 macos"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a>macOS에 Azure CLI 2.0 설치

macOS 플랫폼의 경우 [homebrew 패키지 관리자](http://brew.sh)를 통해 또는 수동으로 Azure CLI를 설치할 수 있습니다. 필요할 때 간편하게 설치, 업데이트 및 제거할 수 있도록 기본 설치 방법으로 homebrew가 사용됩니다.

## <a name="use-homebrew-to-install"></a>homebrew를 사용하여 설치

Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다. 설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다. `apt` 또는 `yum` 같은 다른 패키지 관리자와 비슷합니다.
시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.

### <a name="install-with-homebrew"></a>homebrew로 설치

brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.

```bash
brew update && brew install azure-cli
```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.

### <a name="update-with-homebrew"></a>homebrew로 업데이트

CLI는 버그 픽스, 향상된 기능, 새로운 기능 및 미리 보기 기능이 정기적으로 업데이트됩니다. 약 2주마다 새 릴리스가 제공됩니다. 로컬 리포지토리 정보를 업데이트한 후 CLI 패키지를 업데이트해야 합니다.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>문제 해결

homebrew를 사용하여 CLI를 설치 또는 업데이트할 때 문제가 발생했습니까? 다음은 발생할 수 있는 몇 가지 일반적인 오류와 그 진단 및 해결 방법입니다.

#### <a name="unable-to-find-python-or-installed-packages"></a>Python 또는 설치된 패키지를 찾을 수 없음

설치에서 Python 또는 설치된 패키지를 찾을 수 없는 경우 부 버전 불일치 또는 homebrew 설치 과정에서 다른 문제가 있는 것일 수 있습니다. CLI는 virtualenv를 사용하지 않으므로 homebrew가 올바른 Python 버전을 찾는 것에 의존합니다. Python 설치를 다시 연결하면 이러한 문제가 해결될 수도 있습니다.

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>CLI 버전 만료

설치된 CLI 버전이 만료된 것일 수도 있다는 생각이 들면 `brew update` 명령, `brew upgrade azure-cli` 명령을 차례로 실행합니다. 이 방법으로도 CLI가 업데이트되지 않는 경우 homebrew 패키지는 일반 릴리스보다 더 늦게 출시될 수 있다는 점에 주의하세요. CLI의 첨단 설치가 필요한 경우 [수동으로 설치](#manage-the-cli-manually)해야 합니다.

### <a name="uninstall-with-homebrew"></a>Homebrew로 제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

homebrew로 설치한 경우 제거 시에도 homebrew를 사용해야 합니다.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>CLI 수동 설치

homebrew를 사용하여 CLI 설치를 자동으로 관리할 수 없거나 하고 싶지 않은 경우 수동으로 설치하면 됩니다.

[Linux 수동 설치 지침](install-azure-cli-linux.md)에 따라 macOS에 수동으로 설치합니다. macOS 10.9 이상 버전에는 필요한 모든 종속성이 포함되어 있습니다.

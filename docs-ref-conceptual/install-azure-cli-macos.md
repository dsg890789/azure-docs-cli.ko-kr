---
title: macOS용 Azure CLI 설치
description: macOS에 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 37358e991f96dd517d169e3b3ac651d513897d6d
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-on-macos"></a>macOS에 Azure CLI 2.0 설치

macOS 플랫폼의 경우 [homebrew 패키지 관리자](http://brew.sh)를 사용하여 Azure CLI를 설치할 수 있습니다. Homebrew를 사용하면 손쉽게 CLI 업데이트 설치를 최신으로 유지할 수 있습니다. CLI 패키지는 macOS 버전 10.9 이상에서 테스트 되었습니다.

## <a name="install"></a>설치

Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다. 설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다.
시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.

brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.

```bash
brew update && brew install azure-cli
```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인 하려면 `az login` 명령을 실행합니다.

```azurecli
az login
```

다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

Homebrew 통해 CLI를 설치하는 경우 문제가 발생하는 경우 몇 가지 공용 오류가 있습니다. 해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Python 또는 설치된 패키지를 찾을 수 없음

설치에서 Python 또는 설치된 패키지를 찾을 수 없는 경우 부 버전 불일치 또는 homebrew 설치 과정에서 발생한 다른 문제가 있을 수 있습니다. CLI는 Python 가상환경을 사용하지 않으므로 올바른 Python 버전을 찾는 것에 의존합니다. Python 설치를 다시 연결하면 이러한 문제가 해결될 수도 있습니다.

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>CLI 버전 1.x가 설치되었습니다

낮은 버전이 설치된 경우 부실한 homebrew 캐시로 인한 것일 수 있습니다. [업데이트](#Update) 지침을 따르세요.

## <a name="update"></a>주 지역에서

CLI는 버그 픽스, 향상된 기능, 새로운 기능 및 미리 보기 기능이 정기적으로 업데이트됩니다. 약 2주마다 새 릴리스가 제공됩니다. 로컬 리포지토리 정보를 업데이트한 후 `azure-cli` 패키지를 업그레이드해야 합니다.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Homebrew를 사용하여 `azure-cli` 패키지를 제거합니다.

```bash
brew uninstall azure-cli
```

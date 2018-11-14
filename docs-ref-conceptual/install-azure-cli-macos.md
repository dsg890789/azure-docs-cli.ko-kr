---
title: macOS용 Azure CLI 설치
description: macOS에 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: a79e5445654a9f339321db18b54e558aa598e19b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222262"
---
# <a name="install-azure-cli-on-macos"></a>macOS에 Azure CLI 설치

macOS 플랫폼의 경우 [homebrew 패키지 관리자](https://brew.sh)를 사용하여 Azure CLI를 설치할 수 있습니다. Homebrew를 사용하면 손쉽게 CLI 업데이트 설치를 최신으로 유지할 수 있습니다. CLI 패키지는 macOS 버전 10.9 이상에서 테스트 되었습니다.

## <a name="install"></a>설치

Homebrew는 CLI 설치를 관리하는 가장 쉬운 방법입니다. 설치, 업데이트 및 제거 하는 편리한 방법을 제공 합니다.
시스템에 homebrew가 없는 경우 [homebrew를 설치](https://docs.brew.sh/Installation.html)한 후 계속 진행하세요.

brew 리포지토리 정보를 업데이트한 후 `install` 명령을 실행하여 CLI를 설치할 수 있습니다.

```bash
brew update && brew install azure-cli
```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

Homebrew 통해 CLI를 설치하는 경우 문제가 발생하는 경우 몇 가지 공용 오류가 있습니다. 여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Python 또는 설치된 패키지를 찾을 수 없음

homebrew 설치 중 사소한 버전 불일치 또는 다른 문제가 있을 수 있습니다. CLI는 Python 가상 환경을 사용하지 않으므로, 설치된 Python 버전을 찾는 것에 의존합니다. 가능한 수정 방법은 프로그램을 설치하고 Homebrew에서 `python3` 종속성을 다시 연결하는 것입니다.

```bash
brew update && brew install python3 && brew upgrade python3
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

## <a name="other-installation-methods"></a>다른 설치 방법

Homebrew를 사용하여 사용자 환경에 Azure CLI를 설치할 수 없는 경우 Linux용 설명서 지침을 사용할 수 있습니다. 이 프로세스는 공식적으로 macOS와 호환되도록 유지되지 않습니다. Homebrew와 같은 패키지 관리자를 사용하는 것이 항상 권장됩니다. 사용할 수 있는 다른 옵션이 없는 경우에만 수동 설치 방법을 사용합니다.

수동 설치 지침은 [Linux에 Azure CLI 수동 설치](install-azure-cli-linux.md)를 참조하세요.

## <a name="next-steps"></a>다음 단계

Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.

> [!div class="nextstepaction"]
> [Azure CLI 시작](get-started-with-azure-cli.md)

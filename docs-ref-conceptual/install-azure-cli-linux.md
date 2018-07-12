---
title: Linux용 Azure CLI 2.0 수동 설치
description: Linux용 Azure CLI 2.0을 수동으로 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dade772f178ed9fd321ff45727aea991acd6d311
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439638"
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Linux에 Azure CLI 2.0 수동 설치

배포에 사용할 수 있는 Azure CLI용 패키지가 없는 경우 언제든지 설치 스크립트를 실행하여 수동으로 CLI를 설치할 수 있습니다.

> [!NOTE]
> CLI용 패키지 관리자를 사용하는 것이 좋습니다 패키지 관리자가 항상 최신 업데이트를 갖추도록 확인하고 CLI 구성 요소의 안정성을 보장합니다. 수동으로 설치하기 전에 배포에 필요한 패키지가 있는지 확인합니다.

## <a name="prerequisites"></a>필수 조건

CLI를 설치하려면 시스템에 다음과 같은 소프트웨어가 필요합니다.

* [Python 2.7 또는 Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>설치 또는 업데이트

CLI를 설치하든 또는 업데이트하는, 전체 설치를 수행해야 합니다. 필수 구성 요소를 모두 갖춘 후에는 `curl`을 실행하여 CLI를 설치할 수 있습니다.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

스크립트를 다운로드해 대신 로컬로 실행할 수 있습니다. 변경 내용을 적용하려면 셸을 다시 시작해야 합니다. 

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

수동 설치 중에 몇 가지 공통 문제가 발견됐습니다. 해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).
### <a name="curl-object-moved-error"></a>"개체 이동됨" curl 오류

`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` 명령을 찾을 수 없음

설치 후 명령을 실행할 수 없는 경우 `bash` 또는 `zsh`를 이용해 셸의 명령 해시 캐시를 지웁니다. 실행

```bash
hash -r
```

한 다음 문제가 해결되었는지 확인합니다.

설치 후 셸을 다시 시작하지 않아도 이 문제가 발생할 수 있습니다. `az` 명령의 위치가 `$PATH`여야 합니다. `az` 명령의 위치는

```bash
<install path>/bin
```

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

설치 시 선택한 위치에서 파일을 직접 삭제하여 CLI를 제거합니다. 기본 설치 위치는 `$HOME`입니다.

1. 설치된 CLI 파일을 제거합니다.

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. `$HOME/.bash_profile` 파일을 수정하여 다음 선을 제거합니다.

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. `bash` 또는 `zsh`를 사용하는 경우 셸의 명령 캐시를 다시 로드합니다.

  ```bash
  hash -r
  ```

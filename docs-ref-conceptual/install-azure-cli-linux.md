---
title: "Linux용 Azure CLI 2.0 수동 설치"
description: "Linux용 Azure CLI 2.0을 수동으로 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure linux, azure 설치 linux"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Linux에 Azure CLI 2.0 수동 설치

배포에 사용할 수 있는 Azure CLI용 패키지가 없는 경우 언제든지 설치 스크립트를 실행하여 수동으로 CLI를 설치할 수 있습니다. 사용 가능한 패키지가 있는 경우 언제나 권장하는 설치 방법입니다.

## <a name="prerequisites"></a>필수 구성 요소

CLI를 설치하려면 시스템에 다음과 같은 소프트웨어가 필요합니다.

* [Python 2.7 또는 Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>수동으로 설치 또는 업데이트

CLI를 설치하든 또는 업데이트하는, 전체 설치를 수행해야 합니다. 필수 구성 요소를 모두 갖춘 후에는 `curl`을 실행하여 CLI를 설치할 수 있습니다.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

원하는 경우 또는 시스템에 `curl`이 없는 경우 스크립트를 다운로드하여 로컬로 실행할 수 있습니다. 변경 내용을 적용하려면 셸을 다시 시작해야 합니다. 설치 후 `az` 명령을 사용하여 CLI를 실행합니다.

## <a name="troubleshooting"></a>문제 해결

### <a name="curl-object-moved-error"></a>"개체 이동됨" curl 오류

`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` 명령을 찾을 수 없음

설치 후 명령을 실행할 수 없는 경우 셸의 명령 해시 캐시를 지워야 할 수도 있습니다. 실행

```bash
hash -r
```

한 다음 문제가 해결되었는지 확인합니다.

설치 후 셸을 다시 시작하지 않아도 이 현상이 발생할 수 있습니다. `az` 명령의 위치가 `$PATH`여야 합니다.

설치 스크립트를 실행하면 다음과 같이 됩니다.

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>수동으로 제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

설치 위치에서 파일을 직접 삭제하여 CLI를 제거할 수 있습니다. `https://aka.ms/InstallAzureCLI` 스크립트를 통해 설치한 경우 설치 당시 설치 위치를 선택하셨을 것입니다. 기본 설치 위치는 `$HOME`입니다.

먼저 설치된 CLI 파일을 제거합니다.

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

그런 다음 `$HOME/.bash_profile` 파일을 수정하여 선을 제거합니다.

```
<install location>/lib/azure-cli/az.completion
```

마지막으로, 셸에서 명령 캐시를 사용하는 경우 명령 캐시를 다시 로드합니다. `bash`및 `zsh` 사용자는 이 단계를 수행해야 합니다.

```bash
hash -r
```

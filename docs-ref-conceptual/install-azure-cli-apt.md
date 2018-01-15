---
title: "apt를 사용하여 Azure CLI 2.0 설치"
description: "apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure apt, azure debian, azure ubuntu"
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
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-apt"></a>apt를 사용하여 Azure CLI 2.0 설치

Ubuntu 또는 Debian처럼 `apt`와 함께 제공되는 배포를 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>설치

1. 원본 목록을 수정합니다.

   - 32비트 시스템

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - 64비트 시스템

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. 다음과 같은 sudo 명령을 실행합니다.

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.

## <a name="update"></a>업데이트

`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> 이렇게 하면 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.
> CLI만 업그레이드하려면 `apt-get install`을 사용하세요.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a>제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

1. `apt-get remove`를 사용하여 제거합니다.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. CLI를 다시 설치할 계획이 없으면 Azure CLI 리포지토리 정보를 제거합니다.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. 불필요한 패키지를 제거합니다.

   ```bash
   sudo apt autoremove
   ```

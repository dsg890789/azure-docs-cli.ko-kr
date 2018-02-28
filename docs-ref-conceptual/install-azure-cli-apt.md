---
title: "apt를 사용하여 Linux에 Azure CLI 2.0 설치"
description: "apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 840e5e7d6531fe92d30235f621e381589266d1d3
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/19/2018
---
# <a name="install-azure-cli-20-with-apt"></a>apt를 사용하여 Azure CLI 2.0 설치

Ubuntu 또는 Debian과 같이 `apt`과(와) 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 64비트 패키지를 사용할 수 있습니다. 이 패키지는 다음 항목에서 테스트되었습니다.

* Ubuntu trusty, xenial 및 artful
* Debian wheezy, jessie 및 stretch

## <a name="install"></a>설치

1. 원본 목록을 수정합니다.

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. 다음과 같은 sudo 명령을 실행합니다.

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.

## <a name="troubleshooting"></a>문제 해결

`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다. 해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).

### <a name="apt-key-fails-with-no-dirmngr"></a>apt-key가 "dirmngr 없음"과 함께 실패

`apt-key` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

이 오류는 `apt-key`에 필요한 구성 요소가 누락되었기 때문에 발생합니다. `dirmngr` 패키지를 설치하면 이 문제를 해결할 수 있습니다.

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a>주 지역에서

`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> 이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.
> CLI만 업그레이드하려면 `apt-get install`을 사용하세요.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

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

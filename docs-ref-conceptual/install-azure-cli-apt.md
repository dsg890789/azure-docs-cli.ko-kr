---
title: apt를 사용하여 Linux에 Azure CLI 2.0 설치
description: apt 패키지 관리자를 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/09/2018
---
## <a name="install"></a>설치

1. 원본 목록을 수정합니다.

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Microsoft 서명 키 가져오기:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > 이 서명 키는 사용되지 않으며 2018년 5월말 대체될 예정입니다. `apt`를 사용하여 계속 업데이트하려면 새 키도 설치해야 합니다.
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. CLI 설치:

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인 하려면 `az login` 명령을 실행합니다.

```azurecli
az login
```

다른 로그인 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다. 해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-fails-with-command-not-found"></a>lsb_release가 “명령을 찾을 수 없음”으로 인해 실패

`lsb_release` 명령을 실행할 때 다음 오류와 유사한 출력이 표시될 수 있습니다.

```output
-bash: lsb_release: command not found
```

이 오류는 lsb_release가 설치되어 있지 않기 때문에 발생합니다. `lsb-release` 패키지를 설치하면 이 문제를 해결할 수 있습니다.

```bash
sudo apt-get install lsb-release
```

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

### <a name="apt-key-hangs"></a>apt-key 중지

포트 11371로 나가는 연결을 차단하는 방화벽 뒤에 있는 경우 `apt-key` 명령이 무기한 중지될 수 있습니다. 방화벽은 나가는 연결을 위해 HTTP 프록시를 사용할 수 있습니다.

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

프록시가 있는지 여부를 모르는 경우 시스템 관리자에게 문의하세요. 프록시에 로그인이 필요하지 않으면 사용자, 암호 및 `@` 토큰은 생략합니다.

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

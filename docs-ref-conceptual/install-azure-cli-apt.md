---
title: apt를 사용하여 Linux에 Azure CLI 설치
description: apt 패키지 관리자를 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343148"
---
# <a name="install-azure-cli-with-apt"></a>apt를 사용하여 Azure CLI 설치

Ubuntu 또는 Debian과 같이 `apt`와 함께 제공되는 배포판을 실행하는 경우, Azure CLI에 x86_64 패키지를 사용할 수 있습니다. 이 패키지는 다음 항목에서 테스트되었습니다.

* Ubuntu trusty, xenial, artful 및 bionic
* Debian wheezy, jessie 및 stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Azure CLI용 패키지는 자체 Python 인터프리터를 설치하고 시스템 Python을 사용하지 않습니다.

## <a name="install"></a>설치

1. 설치 프로세스에 필요한 패키지를 가져옵니다.

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. Microsoft 서명 키를 다운로드하고 설치합니다.

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Azure CLI 소프트웨어 리포지토리를 추가합니다.

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. 리포지토리 정보를 업데이트하고 `azure-cli` 패키지를 설치합니다.

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

`az` 명령을 사용하여 Azure CLI를 실행합니다. 로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

`apt`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다. 여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>lsb_release가 올바른 기본 배포 버전을 반환하지 않습니다.

Linux Mint 같은 일부 Ubuntu 또는 Debian 파생 배포판은 `lsb_release`로부터 올바른 버전 이름을 반환하지 않을 수 있습니다. 이 값은 설치 과정에서 패키지 설치를 확인하는 데 사용됩니다. 배포본이 파생된 Ubuntu 또는 Debian 버전의 코드 이름을 알고 있다면 [리포지토리를 추가](#set-release)할 때 수동으로 `AZ_REPO` 값을 설정할 수 있습니다. 그렇지 않은 경우 귀하의 배포에 대해 기본 배포 코드 이름을 확인하고 `AZ_REPO`를 올바른 값으로 설정 하는 방법에 대해 알아봅니다.

### <a name="no-package-for-your-distribution"></a>배포에 필요한 패키지가 없음

배포본이 릴리스된 후에 Azure CLI 패키지가 제공되기까지는 어느 정도 시간이 걸릴 수 있습니다. Azure CLI는 향후 버전의 종속성에 대해 탄력성을 갖도록 설계되었으며 가능한 한 적게 의존합니다. 기본 배포에 사용할 수 있는 패키지가 없는 경우 이전 배포 패키지를 시도합니다.

이를 위해, [리포지토리를 추가](#set-release)할 때 수동으로 `AZ_REPO` 값을 설정합니다. Ubuntu 배포의 경우 `bionic` 리포지토리를 사용하고 Debian 배포판의 경우 `stretch`를 사용합니다. Ubuntu Trusty 및 Debian Wheezy 이전에 릴리스된 배포는 지원되지 않습니다.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>주 지역에서

`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> 이 명령은 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.
> CLI만 업그레이드하려면 `apt-get install`을 사용하세요.
> 
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

3. 서명 키를 제거합니다.

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. 불필요한 패키지를 제거합니다.

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>다음 단계

Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.

> [!div class="nextstepaction"]
> [Azure CLI 시작](get-started-with-azure-cli.md)

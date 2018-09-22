---
title: zypper를 사용하여 Linux에 Azure CLI 2.0 설치
description: zypper를 사용하여 Azure CLI 2.0을 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d5197e1d62b89bc293970a85bcf976a38898862e
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46469915"
---
# <a name="install-azure-cli-20-with-zypper"></a>zypper를 사용하여 Azure CLI 2.0 설치

openSUSE 또는 SLES 등의 `zypper`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다. 이 패키지는 openSUSE 42.2 및 SLES 12 SP 2와 함께 테스트되었습니다.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>설치

1. `curl` 설치:

   ```bash
   sudo zypper install -y curl
   ```

2. Microsoft 리포지토리 키를 가져옵니다.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. 로컬 `azure-cli` 리포지토리 정보를 만듭니다.

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. `zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

다른 인증 방법에 대한 자세한 내용은 [Azure CLI 2.0으로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="update"></a>주 지역에서

`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. 시스템에서 패키지를 제거합니다.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. 리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

## <a name="next-steps"></a>다음 단계

Azure CLI를 설치한 후 해당 기능 및 일반 명령을 잠시 둘러보세요.

> [!div class="nextstepaction"]
> [Azure CLI 시작](get-started-with-azure-cli.md)

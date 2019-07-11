---
title: zypper를 사용하여 Linux에 Azure CLI 설치
description: zypper를 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f8a3bec4fffb731c6521fa7b8a2a90798ef191e6
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516259"
---
# <a name="install-azure-cli-with-zypper"></a>zypper를 사용하여 Azure CLI 설치

openSUSE 또는 SLES 등의 `zypper`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다. 이 패키지는 openSUSE 42.2 이상 및 SLES 12 SP 2 이상에서 테스트되었습니다.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

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

다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

`zypper`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다. 여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>프록시 연결 차단

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

`yast2`를 통해 이 프록시를 항상 사용하도록 명시적으로 `zypper`를 구성할 수도 있습니다. 이렇게 하려면 `yast2 proxy` 명령을 슈퍼 사용자 권한으로 실행하고 양식에 제공된 정보를 입력합니다. 시스템에서 창 관리자를 사용할 수 있으면 `YaST Control Center`에서 `Network Services > Proxy` 창을 사용할 수도 있습니다.

고급 구성 또는 자세한 내용은 [openSUSE 프록시 구성 설명서](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)를 참조하세요.

Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update">업데이트</a>	

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

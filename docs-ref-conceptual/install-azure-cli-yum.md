---
title: yum을 사용하여 Linux에 Azure CLI 설치
description: yum을 사용하여 Azure CLI를 설치하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bc3ae41ea04ae8d7f62242b2bfe415c8a3bfea33
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516291"
---
# <a name="install-azure-cli-with-yum"></a>yum을 사용하여 Azure CLI 설치

RHEL, Fedora, CentOS 등의 `yum`를 사용하는 Linux 배포의 경우, Azure CLI에서 사용할 수 있는 패키지가 있습니다. 이 패키지는 RHEL 7, Fedora 19 이상, CentOS 7를 사용하여 테스트 되었습니다.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>설치

1. Microsoft 리포지토리 키를 가져옵니다.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. 로컬 `azure-cli` 리포지토리 정보를 만듭니다.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. `yum install` 명령을 사용하여 설치됩니다.

   ```bash
   sudo yum install azure-cli
   ```

그런 다음 `az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다. 로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.

## <a name="troubleshooting"></a>문제 해결

`yum`을 사용해 설치할 때 몇 가지 일반적인 문제가 여기에 표시됩니다. 여기에서 다루지 않는 문제가 발생하는 경우, [github에 문제를 제출합니다](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>프록시 연결 차단

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

이 프록시를 항상 사용하도록 명시적으로 `yum`을 구성할 수도 있습니다. `/etc/yum.conf`의 `[main]` 섹션 아래에 다음 줄이 표시되는지 확인합니다.

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

Microsoft 서명 키를 가져오고 리포지토리에서 패키지를 가져오려면 프록시에서 다음 주소에 대한 HTTPS 연결을 허용해야 합니다.

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update">업데이트</a>

`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. 시스템에서 패키지를 제거합니다.

   ```bash
   sudo yum remove azure-cli
   ```

2. CLI를 다시 설치하지 않으려면 리포지토리 정보를 제거합니다.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
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

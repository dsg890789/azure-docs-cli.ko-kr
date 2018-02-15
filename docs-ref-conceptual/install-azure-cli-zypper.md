---
title: "zypper를 사용하여 Linux에 Azure CLI 2.0 설치"
description: "zypper를 사용하여 Azure CLI 2.0을 설치하는 방법"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6ee3aff74f43fab0c80c58c7fe57c9fa74a6ef2f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>zypper를 사용하여 Azure CLI 2.0 설치

openSUSE 또는 SLES 등의 `zypper`과 함께 제공되는 배포를 실행하는 경우 Azure CLI에서 사용할 수 있는 패키지가 있습니다. 이 패키지는 openSUSE 42.2 및 SLES 12 SP 2와 함께 테스트되었습니다.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>설치

1. `curl` 설치:

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Microsoft 리포지토리 키를 가져옵니다.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. 로컬 `azure-cli` 리포지토리 정보를 만듭니다.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. `zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

`az` 명령을 사용하여 Azure CLI를 실행할 수 있습니다.

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
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. 리포지토리 정보를 제거한 경우 Microsoft GPG 서명 키도 제거합니다.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```


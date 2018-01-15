---
title: "zypper를 사용하여 Azure CLI 2.0 설치"
description: "zypper를 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "azure cli, azure cli 설치, azure cli zypper, azure cli opensuse, azure cli sle"
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
ms.openlocfilehash: 6b9a97e73f45c8271f1e8f19d5a8cf5f9f748d07
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>zypper를 사용하여 Azure CLI 2.0 설치

OpenSUSE 또는 SLE처럼 `zypper`와 함께 제공되는 배포를 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.

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

## <a name="update"></a>업데이트

`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

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


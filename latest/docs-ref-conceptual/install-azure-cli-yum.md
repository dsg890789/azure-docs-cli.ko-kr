---
title: "yum을 사용하여 Azure CLI 2.0 설치"
description: "yum을 사용하여 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure yum,azure rhel, azure fedora, azure centos"
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
ms.openlocfilehash: de695454c6f3109679b9eb9f6c0d77348d354518
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-yum"></a>yum을 사용하여 Azure CLI 2.0 설치

RHEL, Fedora 또는 CentOS처럼 `yum`과 함께 제공되는 배포판을 실행하는 경우 시스템에 설치할 수 있는Azure CLI용 패키지가 제공됩니다.

> [!NOTE]
> CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다. 배포에 패키지가 없으면 [Python](https://www.python.org/downloads/)을 설치하세요.

## <a name="install"></a>설치 

1. Microsoft 리포지토리 키를 가져옵니다.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. 로컬 `azure-cli` 리포지토리 정보를 만듭니다.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. `yum` 패키지 인덱스를 업데이트하고 다음을 설치합니다.

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

`az` 명령을 사용하여 Azure CLI를 실행합니다.

## <a name="update"></a>업데이트

`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

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

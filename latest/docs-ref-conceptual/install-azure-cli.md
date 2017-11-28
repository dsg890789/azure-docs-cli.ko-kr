---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0 설치에 대한 참조 문서입니다."
keywords: "Azure CLI, Azure CLI 설치, Azure Python CLI, Azure CLI 참조"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 2b56382355cad5313a604ed1f493a2bcbebf3e27
ms.sourcegitcommit: e9b4c6dd9093980b69ca47f93f44ac54d0e5b68a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/03/2017
---
# <a name="install-azure-cli-20"></a>Azure CLI 2.0 설치

지금 새 버전의 Azure CLI를 설치하세요.
Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트 되었습니다.
macOS, Linux 및 Windows에서 사용할 수 있습니다.
최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.

> [!NOTE]
> 이전 버전의 Azure CLI가 필요한 경우 [Azure CLI 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>macOS에 설치

macOS에서는 [Homebrew](https://brew.sh/) 또는 수동으로 설치할 수 있습니다.

### <a name="install-with-homebrew"></a>Homebrew로 설치

1. 아직 설치하지 않은 경우 [Homebrew 설치 지침](https://docs.brew.sh/Installation.html)에 따라 Homebrew를 설치하십시오.

2. 이전에 CLI를 수동으로 설치한 경우 [수동 제거](#UninstallManually) 지침을 따르세요.

3. 로컬 Homebrew 리포지토리를 업데이트합니다.

   ```bash
   brew update
   ```

4. `azure-cli` 패키지를 설치합니다.

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> 이전에 Azure CLI 1.0을 Homebrew로 설치한 경우 패키지를 설치하는 대신 정기적인 Homebrew 업데이트 프로세스를 통해 CLI 2.0을 확보할 수 있습니다.
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a>수동 설치

1. `curl`을 사용하여 Azure CLI 2.0을 설치합니다.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. 일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.

   ```bash
   exec -l $SHELL
   ```
   
3. 명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="install-on-windows"></a>Windows에 설치

### <a name="install-with-msi-for-the-windows-command-line"></a>Windows 명령줄용 MSI를 사용하여 설치 

Windows에 CLI를 설치하고 Windows 명령줄에서 사용하려면 [Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다운로드하여 실행합니다.

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Windows 내 Ubuntu에 있는 Bash에서 apt-get을 사용하여 설치

1. Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.

2. Bash 셸을 엽니다.

3. 소스 목록을 수정합니다.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. 다음과 같은 sudo 명령을 실행합니다.

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="install-with-apt-package-manager"></a>apt 패키지 관리자를 사용하여 설치 

Ubuntu 또는 Debian과 같은 `apt` 패키지 관리자를 사용하는 배포판의 경우 `apt-get`을 통해 Azure CLI 2.0을 설치할 수 있습니다.

> [!NOTE]
> CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다. 배포판에 패키지가 없으면 [Python을 설치](https://www.python.org/downloads/)합니다.

1. 소스 목록을 수정합니다.
 
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

3.  명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="install-with-yum-package-manager"></a>yum 패키지 관리자를 사용하여 설치

Red Hat Enterprise Linux(RHEL), Fedora 또는 CentOS와 같은 `yum` 패키지 관리자를 사용하는 배포판의 경우 `yum`를 통해 Azure CLI 2.0을 설치할 수 있습니다.

> [!NOTE]
> CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다. 배포에 패키지가 없으면 [Python을 설치](https://www.python.org/downloads/)합니다.

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

4. 명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="install-with-zypper-package-manager"></a>zypper 패키지 관리자를 사용하여 설치

OpenSUSE 또는 SLE와 같은 `zypper` 패키지 관리자를 사용하는 배포판의 경우 `zypper`를 통해 Azure CLI 2.0을 설치할 수 있습니다.

> [!NOTE]
> CLI를 사용하려면 Python 2.7.x 또는 Python 3.x가 있어야 합니다. 배포에 패키지가 없으면 [Python을 설치](https://www.python.org/downloads/)합니다.

1. Microsoft 리포지토리 키를 가져옵니다.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. 로컬 `azure-cli` 리포지토리 정보를 만듭니다.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. `zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. 명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="install-with-docker"></a>Docker를 사용하여 설치

Azure CLI 2.0을 포함하여 미리 구성된 Docker 이미지를 유지하고 있습니다.

`docker run`을 사용하여 CLI를 설치합니다.

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.

CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.

> [!NOTE]
> 사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 마운트할 수 있습니다.

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><a name="Linux"/>패키지 관리자를 사용하지 않고 Linux에 설치

가능한 경우 패키지 관리자를 사용하여 CLI를 설치하는 것이 좋습니다. Microsoft의 리포지토리를 추가하지 않거나 제공된 패키지가 없는 배포로 작업하는 경우에 CLI을 수동으로 설치할 수 있습니다.

1. Linux 배포판에 따라 필수 구성 요소를 설치합니다.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

배포판이 위에 나열되지 않은 경우 [Python 2.7 이상](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) 및 [OpenSSL](https://www.openssl.org/source/)을 설치해야 합니다.

2. `curl`을 사용하여 CLI를 설치합니다.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. 일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.

   ```bash
   exec -l $SHELL
   ```

4. 명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.

## <a name="troubleshooting"></a>문제 해결

CLI 설치 중에 문제가 발생하면 이 섹션을 확인하여 해당 사례가 적용되는지 확인합니다. 해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>"개체 이동됨" curl 오류

`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` 명령을 찾을 수 없음

셸의 명령 해시 캐시를 지워야 할 수 있습니다. 실행

```bash
hash -r
```

한 다음 문제가 해결되었는지 확인합니다. `$PATH`에 명령이 없을 수도 있습니다. `$PATH`에 `<install path>/bin`이 표시되는지 확인하고, 필요한 경우 셸을 다시 시작합니다.

## <a name="uninstall-cli-1x-versions"></a>CLI 1.x 버전 제거

시스템에서 이전의 CLI 1.x 버전을 사용할 수 있는 경우 사용된 설치 유형에 따라 이를 제거할 수 있습니다.

### <a name="uninstall-with-npm"></a>npm을 사용하여 제거

`npm uninstall`을 사용하여 이전 버전의 CLI를 제거합니다.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a>배포판 패키지를 사용하여 제거

[Azure CLI 설치 관리자(MSI)](http://aka.ms/webpi-azure-cli) 또는 [macOS 패키지](http://aka.ms/mac-azure-cli)를 통해 설치한 경우 동일한 도구를 사용하여 설치를 제거합니다.

### <a name="uninstall-with-docker"></a>Docker를 사용하여 제거

Docker 이미지를 설치하여 이전 버전의 CLI를 사용한 경우 해당 이미지 및 관련 컨테이너를 제거합니다. 그런 다음 설치 지침에서 설명하는 대로 새 Docker 이미지를 설치한 후 컨테이너를 다시 만들 수 있습니다.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>CLI 업데이트

Azure CLI를 업데이트하려면 설치하는 데 사용했던 것과 동일한 방법을 사용합니다.

### <a name="update-with-homebrew"></a>Homebrew로 업데이트

1. 이전에 수동으로 설치한 경우 [Homebrew로 설치](#macOS) 지침을 따르세요.

2. 로컬 Homebrew 리포지토리 정보를 업데이트합니다.

   ```bash
   brew update
   ```

3. 설치된 패키지를 업그레이드합니다.

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a>MSI를 사용하여 업데이트

[Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다시 실행합니다.

### <a name="update-with-apt"></a>apt를 사용하여 업데이트

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

### <a name="update-with-yum"></a>yum을 사용하여 업데이트

`yum update` 명령을 사용하여 Azure CLI를 업데이트합니다.

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a>zypper를 사용하여 업데이트

`zypper update` 명령을 사용하여 패키지를 업데이트할 수 있습니다.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a>Docker를 사용하여 업데이트

1. `docker pull`을 사용하여 로컬 이미지를 업데이트합니다.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. 현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> 특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.

3. 컨테이너를 중지하고 다시 만듭니다.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>수동으로 업데이트

[macOS](#macOS) 또는 [Linux](#Linux)에 대한 수동 설치 지침에 따라 업데이트합니다.

## <a name="uninstall"></a>제거

CLI를 제거하려는 경우 유감스럽게 생각합니다. CLI를 설치하는 데 사용한 동일한 방법을 사용하여 제거해야 합니다.

### <a name="uninstall-with-homebrew"></a>Homebrew로 제거

`azure-cli` 패키지를 제거합니다.

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a>MSI를 사용하여 제거

[MSI](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.

### <a name="uninstall-with-apt"></a>apt를 사용하여 제거

`apt-get remove`를 통해 제거합니다.

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a>yum을 사용하여 제거

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
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a>zypper를 사용하여 제거

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
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a>Docker를 사용하여 제거

Docker 이미지를 설치한 경우 이를 실행하는 컨테이너를 모두 제거한 다음 로컬 이미지를 삭제해야 합니다.

1. azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. CLI 이미지가 있는 컨테이너를 모두 삭제합니다.

   ```bash
   docker rm 34a868beb2ab
   ```

3. 로컬로 설치된 CLI 이미지를 제거합니다.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> 특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><a name="UninstallManually"/>수동으로 제거

https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.

1. 설치된 파일을 제거합니다.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. `<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.

3. 셸에서 명령 캐시를 사용하는 경우 다시 로드합니다.

   ```bash
   hash -r
   ```

> [!Note]
> 기본 설치 위치는 macOS의 경우 `/Users/<username>`, Linux의 경우 `/home/<username>` 입니다.

## <a name="report-cli-issues-and-feedback"></a>CLI 문제 보고 및 피드백

도구에서 버그가 발생하면 GitHub 리포지토리의 [Issues](https://github.com/Azure/azure-cli/issues) 섹션에서 문제를 제출해 주세요.
명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 주세요.

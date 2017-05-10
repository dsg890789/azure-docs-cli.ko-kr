---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0에 대한 참조 문서"
keywords: "Azure CLI 2.0, Azure CLI 2.0 참조, Azure CLI 2.0 설치, Azure Python CLI, Azure CLI 2.0 제거"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 664535701ad814f8ff85fefe8ecc45772777d0ba
ms.sourcegitcommit: ec22ff07aedb5c47e5f636f2a9a341c3edbe7ca1
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="install-azure-cli-20"></a>Azure CLI 2.0 설치

지금 새 버전의 Azure CLI를 설치하세요.
Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.
macOS, Linux 및 Windows에서 사용할 수 있습니다.
최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.

> [!NOTE]
> 이전 버전의 Azure CLI가 필요할 경우 [Azure 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.

## <a name="macos"></a>macOS

1. `curl` 명령 하나로 Azure CLI 2.0을 설치합니다.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. 일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.

   ```bash
   exec -l $SHELL
   ```
   
3. 명령 프롬프트에서 `az` 명령을 사용하여 Azure CLI 2.0을 실행합니다.

> [!Note]
> InstallAzureCli를 함께 설치할 경우 `az component update`가 지원되지 않습니다.
> 최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.
> 
> 제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.

## <a name="windows"></a>Windows

Azure CLI 2.0은 Bash 명령 구문을 지원하므로 Windows에서 CLI를 사용할 때 Ubuntu의 Bash를 유용하게 사용할 수 있습니다.
Bash를 사용하지 않는 경우 Windows 명령줄에서 CLI를 설치하고 사용할 수 있습니다.

### <a name="bash-on-ubuntu-on-windows"></a>Windows에서 Ubuntu의 Bash

1. Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.

2. Bash 셸을 엽니다.

3. 소스 목록을 수정합니다.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. 다음과 같은 sudo 명령을 실행합니다.

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> apt-get을 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.
> CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.
> 
> 제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.

### <a name="windows-command-line"></a>Windows 명령줄 

1. Python 사이트를 방문하고 Windows용 [Python을 다운로드](https://www.python.org/downloads/)합니다.
   Python을 설치할 때는 Pip 구성 요소를 설치해야 합니다.
   설치가 완료되면 Python을 PATH 환경 변수에 추가합니다(설치 관리자가 관련 메시지를 표시합니다).

2. 명령 프롬프트에서 Python 설치를 확인합니다.

   ```bash
   python --version
   ```

3. `pip`를 사용하여 Azure CLI 2.0을 설치합니다.

   ```bash
   pip install --user azure-cli
   ```

4. az.bat가 포함된 폴더를 경로에 추가합니다.
   CLI `az.bat`는 `%USERPROFILE%\AppData\Roaming\Python\Scripts` 또는 `%USERPROFILE%\AppData\Roaming\Python\PythonXY\Scripts`에 설치될 수 있습니다. 여기서 `XY`는 Python 버전입니다(예: `%USERPROFILE%\AppData\Roaming\Python\Python27\Scripts`).
   `az.bat`가 포함된 폴더를 경로에 추가합니다.
   
4. 명령 프롬프트에서 `az` 명령을 사용하여 Azure CLI 2.0을 실행합니다.

> [!NOTE]
> Azure CLI 2.0이 이미 설치되어 있고 최신 버전인지 확인하려는 경우 `az --version`을 사용하여 사용 중인 버전을 확인하세요.
> 이 버전을 [https://pypi.python.org/pypi/azure-cli](https://pypi.python.org/pypi/azure-cli)에 제공되는 최신 버전과 비교해 보세요.
> 
> 최신 CLI로 업데이트하려면 `az component update`를 실행하세요.
> 
> CLI를 제거하려면 `pip uninstall azure-cli`를 실행하세요.

## <a name="linux"></a>Linux

1. Linux에서는 특정 [필수 구성 요소](#linux-prerequisites)를 설치해야 할 수 있습니다.

2. `curl` 명령 하나로 Azure CLI 2.0을 설치합니다.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. 일부 변경 내용을 적용하기 위해 명령 셸을 다시 시작해야 할 수 있습니다.

   ```bash
   exec -l $SHELL
   ```

4. 명령 프롬프트에서 `az` 명령을 사용하여 Azure CLI 2.0을 실행합니다.

> [!Note]
> InstallAzureCli를 함께 설치할 경우 `az component update`가 지원되지 않습니다.
> 최신 CLI로 업데이트하려면 `curl -L https://aka.ms/InstallAzureCli | bash`를 다시 실행하세요.
> 
> 제거하려면 [수동 제거 지침](#uninstall)을 참조하세요.

## <a name="docker"></a>Docker

Microsoft는 Azure CLI로 미리 구성된 Docker 이미지를 유지합니다.

`docker run`을 사용하여 Azure CLI를 설치합니다.

```bash
docker run azuresdk/azure-cli-python:<version>
```

[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.

> [!NOTE]
> 사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> Docker 이미지는 [`component` 기능](/cli/azure/component)을 지원하지 않습니다.
> Azure CLI 2.0을 업데이트하려면 `docker run`을 사용하여 최신 이미지 또는 원하는 특정 이미지를 설치하세요.

## <a name="apt-get"></a>apt-get

Debian/Ubuntu 기반 시스템의 경우 `apt-get`를 통해 Azure CLI 2.0을 설치할 수 있습니다.

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
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> apt-get을 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.
> CLI를 업데이트하려면 `sudo apt-get update && sudo apt-get install azure-cli`를 다시 실행합니다.
> 
> 제거하려면 `sudo apt-get remove azure-cli`를 실행합니다.

## <a name="linux-prerequisites"></a>Linux 필수 구성 요소

1. [Python](https://www.python.org/downloads)이 없을 경우 설치하세요.

2. Linux 배포에 따라 필수 구성 요소를 설치하세요.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a>문제 해결
-------------------------------

### <a name="errors-with-curl-redirection"></a>curl 리디렉션 관련 오류

`curl` 명령에서 `-L` 매개 변수와 관련한 오류나 "개체 이동됨"이라는 오류가 발생할 경우 aka.ms url 대신 전체 url을 사용해 보세요.

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```


### <a name="errors-on-install-with-cffi-or-cryptography"></a>`cffi`를 사용한 설치 또는 암호화 시 오류

OS X에 설치 시 오류가 발생 하는 경우 `pip`를 업그레이드하세요.

```bash
pip install --upgrade --force-reinstall pip
```

**Debian** 또는 **Ubuntu**에서 설치 시 이 예와 같은 오류가 발생할 경우 `libssl-dev` 및 `libffi-dev`를 설치하세요.

```bash
sudo apt-get update
sudo apt-get install -y libssl-dev libffi-dev
```

또한 사용 중인 Python 버전에 맞는 Python Dev도 설치하세요.

Python 2:

```bash
sudo apt-get install -y python-dev
```

Python 3:

```bash
sudo apt-get install -y python3-dev
```

Ubuntu 15의 경우 `build-essential`도 필요할 수 있습니다.

```bash
sudo apt-get install -y build-essential
```

### <a name="example-errors"></a>오류 예

```
Downloading cffi-1.5.2.tar.gz (388kB)
    100% |################################| 389kB 3.9MB/s
    Complete output from command python setup.py egg_info:

        No working compiler found, or bogus compiler options
        passed to the compiler from Python's distutils module.
        See the error messages above.
        (If they are about -mno-fused-madd and you are on OS/X 10.8,
        see http://stackoverflow.com/questions/22313407/ .)

    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-77i2fido/cffi/
```

```
#include <openssl/e_os2.h>
                            ^
compilation terminated.
error: command 'x86_64-linux-gnu-gcc' failed with exit status 1

Failed building wheel for cryptography
```

Stack Overflow 질문 참조 - [PIP 및 setup.py를 사용하여 Python 암호화 패키지를 설치하지 못했습니다.](http://stackoverflow.com/questions/22073516/failed-to-install-python-cryptography-package-with-pip-and-setup-py)

## <a name="uninstall"></a>제거

https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.

1. 설치된 파일을 제거합니다.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. `<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.

> [!Note]
> 기본 설치 위치는 `/Users/<username>`입니다.

pip, apt-get 또는 Docker를 사용하여 CLI를 설치한 경우 동일한 도구를 사용하여 제거하세요.

## <a name="reporting-issues-and-feedback"></a>문제 보고 및 피드백

도구에서 버그가 발견되면 GitHub 리포지토리의 [문제](https://github.com/Azure/azure-cli/issues) 섹션에 문제를 기록해 주세요.
명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 보세요.

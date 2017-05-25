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
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/16/2017
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

MSI를 사용하여 CLI를 설치하고 Windows 명령줄에서 사용하거나 Windows의 Ubuntu에 있는 Bash에서 apt-get을 사용하여 CLI를 설치할 수 있습니다.

### <a name="msi-for-the-windows-command-line"></a>Windows 명령줄용 MSI 

Windows에서 CLI를 설치하고 Windows 명령줄에서 사용하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다운로드한 후 실행합니다.

> [!NOTE]
> MSI를 사용하여 설치하는 경우 `az component`가 지원되지 않습니다.
> 최신 CLI로 업데이트하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하세요.
> 
> CLI를 제거하려면 [msi](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>Windows의 Ubuntu에 있는 Bash의 apt-get

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

apt-get, Docker 또는 msi를 사용하여 CLI를 설치한 경우 동일한 도구를 사용하여 제거하세요.

## <a name="reporting-issues-and-feedback"></a>문제 보고 및 피드백

도구에서 버그가 발견되면 GitHub 리포지토리의 [문제](https://github.com/Azure/azure-cli/issues) 섹션에 문제를 기록해 주세요.
명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 보세요.

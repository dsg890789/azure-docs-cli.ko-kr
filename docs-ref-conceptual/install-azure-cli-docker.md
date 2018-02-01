---
title: "Docker와 함께 Azure CLI 설치"
description: "Azure CLI 2.0과 함께 Docker 컨테이너를 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure docker,azure docker 이미지,"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 7a12da712cd2aad5bb5fb56e27267a8e05df34a6
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/31/2018
---
# <a name="install-azure-cli-20-with-docker"></a>Docker를 사용하여 Azure CLI 2.0 설치

Docker를 사용하여 Azure CLI 2.0이 사전 설치된 독립 실행형 Linux 컨테이너를 설치할 수 있습니다. 그러면 CLI를 사용해보고 자신에게 적합한지 확인할 수 있는 환경을 신속하게 시작하거나, 기본 이미지로 사용할 수 있습니다.

## <a name="install-with-docker"></a>Docker를 사용하여 설치

`docker run`을 사용하여 CLI를 설치합니다.

   ```bash
   docker run -it microsoft/azure-cli:<version>
   ```

[Docker 태그](https://hub.docker.com/r/microsoft/azure-cli/tags/)를 통해 사용 가능한 버전을 확인합니다.

CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.

> [!NOTE]
> 사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli:<version>
> ```

### <a name="update-with-docker"></a>Docker를 사용하여 업데이트

Docker를 사용하여 업데이트하려면 새 이미지를 풀링하고 모든 기존 컨테이너를 다시 만들어야 합니다. 이러한 이유로 CLI를 데이터 저장소로로 호스트하는 컨테이너를 사용하지 말아야 합니다.

1. `docker pull`을 사용하여 로컬 이미지를 업데이트합니다.

   ```bash
   docker pull microsoft/azure-cli
   ```

2. 현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > 특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.

3. 컨테이너를 중지하고 다시 만듭니다.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run microsoft/azure-cli
   ```

### <a name="uninstall-with-docker"></a>Docker를 사용하여 제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

CLI Docker 이미지를 적절하게 제거하려면 이미지에서 실행 중인 컨테이너를 모두 제거한 후 로컬 이미지를 삭제해야 합니다.

1. azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > 특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.

2. CLI 이미지가 있는 컨테이너를 모두 삭제합니다.

   ```bash
   docker rm 34a868beb2ab
   ```

3. 로컬로 설치된 CLI 이미지를 제거합니다.

   ```bash
   docker rmi microsoft/azure-cli
   ```


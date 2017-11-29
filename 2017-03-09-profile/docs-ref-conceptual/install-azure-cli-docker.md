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
ms.openlocfilehash: 76ecf2c9cd0e6e694a31ac160112d1348863f118
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-docker"></a><span data-ttu-id="306fd-104">Docker를 사용하여 Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="306fd-104">Install Azure CLI 2.0 with Docker</span></span>

<span data-ttu-id="306fd-105">Docker를 사용하여 Azure CLI 2.0이 사전 설치된 독립 실행형 Linux 컨테이너를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-105">You can use Docker to install a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="306fd-106">그러면 CLI를 사용해보고 자신에게 적합한지 확인할 수 있는 환경을 신속하게 시작하거나, 기본 이미지로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-106">This lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or allows you to use this as a base image.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="306fd-107">Docker를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="306fd-107">Install with Docker</span></span>

<span data-ttu-id="306fd-108">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="306fd-109">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-109">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="306fd-110">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="306fd-111">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

### <a name="update-with-docker"></a><span data-ttu-id="306fd-112">Docker를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="306fd-112">Update with Docker</span></span>

<span data-ttu-id="306fd-113">Docker를 사용하여 업데이트하려면 새 이미지를 풀링하고 모든 기존 컨테이너를 다시 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="306fd-114">이러한 이유로 CLI를 데이터 저장소로로 호스트하는 컨테이너를 사용하지 말아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-114">For this reason you should try and avoid using a container which hosts the CLI as a data store.</span></span>

1. <span data-ttu-id="306fd-115">`docker pull`을 사용하여 로컬 이미지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-115">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="306fd-116">현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-116">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > <span data-ttu-id="306fd-117">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-117">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="306fd-118">컨테이너를 중지하고 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-118">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="306fd-119">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="306fd-119">Uninstall with Docker</span></span>

<span data-ttu-id="306fd-120">Azure CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-120">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="306fd-121">제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-121">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="306fd-122">버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-122">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="306fd-123">또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-123">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="306fd-124">CLI Docker 이미지를 적절하게 제거하려면 이미지에서 실행 중인 컨테이너를 모두 제거한 후 로컬 이미지를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-124">To properly uninstall the CLI Docker image you need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="306fd-125">azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-125">Get the containers running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > <span data-ttu-id="306fd-126">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-126">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

2. <span data-ttu-id="306fd-127">CLI 이미지가 있는 컨테이너를 모두 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-127">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="306fd-128">로컬로 설치된 CLI 이미지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="306fd-128">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```


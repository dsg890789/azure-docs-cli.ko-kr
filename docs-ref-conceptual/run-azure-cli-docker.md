---
title: Docker 컨테이너에서 Azure CLI 실행
description: Azure CLI를 호스팅하는 Docker 컨테이너 실행 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40e6865ce07b6ccb8e84a2666f0bcd6df3b5cfcf
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177762"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="f5473-103">Docker 컨테이너에서 Azure CLI 실행</span><span class="sxs-lookup"><span data-stu-id="f5473-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="f5473-104">Docker를 사용하여 Azure CLI가 사전 설치된 독립 실행형 Linux 컨테이너를 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="f5473-105">Docker로 CLI를 실행하는 격리 환경을 신속하게 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="f5473-106">이미지를 배포를 위한 베이스로 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="f5473-107">Docker 컨테이너에서 실행</span><span class="sxs-lookup"><span data-stu-id="f5473-107">Run in a Docker container</span></span>

<span data-ttu-id="f5473-108">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="f5473-109">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}/.ssh:/root/.ssh`를 사용하여 SSH 키를 환경에 탑재합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="f5473-110">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="f5473-111">로그인하려면, [az login](/cli/azure/reference-index#az-login) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f5473-112">다른 인증 방법에 대한 자세한 내용은 [Azure CLI로 로그인](authenticate-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f5473-112">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="f5473-113">Docker 이미지 업데이트</span><span class="sxs-lookup"><span data-stu-id="f5473-113">Update Docker image</span></span>

<span data-ttu-id="f5473-114">Docker를 사용하여 업데이트하려면 새 이미지를 풀링하고 모든 기존 컨테이너를 다시 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="f5473-115">이러한 이유로 CLI를 데이터 저장소로 호스트하는 컨테이너를 사용하지 말아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="f5473-116">`docker pull`을 사용하여 로컬 이미지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="f5473-117">Docker 이미지 제거</span><span class="sxs-lookup"><span data-stu-id="f5473-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f5473-118">CLI 이미지를 실행하는 모든 컨테이너를 중지한 후 이미지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f5473-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="f5473-119">다음 단계</span><span class="sxs-lookup"><span data-stu-id="f5473-119">Next Steps</span></span>

<span data-ttu-id="f5473-120">Azure CLI를 사용할 준비가 되었으면 해당 기능 및 일반 명령을 잠시 둘러보세요.</span><span class="sxs-lookup"><span data-stu-id="f5473-120">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f5473-121">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="f5473-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

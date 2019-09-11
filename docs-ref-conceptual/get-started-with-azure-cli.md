---
title: Azure CLI 시작
description: 명령 기본 사항을 학습하여 Azure CLI 사용을 시작합니다.
keywords: Azure CLI, CLI 도움말, Azure 도움말, 쿼리, 자동화,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c667f6fa00d8a03b6a451728ffcc1da3e446a741
ms.sourcegitcommit: f9bfb4b063151434b3a9bff936a73b251666e775
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/10/2019
ms.locfileid: "70878249"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="25687-104">Azure CLI 시작</span><span class="sxs-lookup"><span data-stu-id="25687-104">Get started with Azure CLI</span></span>

<span data-ttu-id="25687-105">Azure CLI 시작!</span><span class="sxs-lookup"><span data-stu-id="25687-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="25687-106">CLI는 특히 자동화 기능을 통해 Azure 서비스를 빠르고 효율적으로 사용할 수 있도록 디자인된 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="25687-107">이 문서에서는 CLI의 여러 기능을 소개하고 생산성 향상에 도움이 되는 리소스에 대한 링크를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

> [!NOTE]
>
> <span data-ttu-id="25687-108">스크립트 및 Microsoft 설명서 사이트에 작성된 Azure CLI 예제는 `bash` 셸용입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="25687-109">한 줄 예제는 모든 플랫폼에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="25687-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="25687-110">연속하는 줄을 포함하는 더 긴 예제 (`\`) 또는 변수 할당은 PowerShell을 포함하여 다른 셸에서 작동하도록 수정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-110">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="25687-111">Azure Cloud Shell에서 설치 또는 실행</span><span class="sxs-lookup"><span data-stu-id="25687-111">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="25687-112">Azure CLI를 시작하는 가장 쉬운 방법은 브라우저를 통해 Azure Cloud Shell 환경에서 실행하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-112">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="25687-113">Cloud Shell에 대해 자세히 알아보려면 [Azure Cloud Shell의 Bash에 대한 빠른 시작](/azure/cloud-shell/quickstart)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="25687-113">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="25687-114">CLI를 설치할 준비가 되었으면 [설치 지침](install-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="25687-114">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="25687-115">CLI가 처음으로 설치되면 `az --version`을 실행하여 CLI가 설치되어 있고 올바른 버전인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-115">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="25687-116">로그인</span><span class="sxs-lookup"><span data-stu-id="25687-116">Sign in</span></span>

<span data-ttu-id="25687-117">로컬 설치에 CLI 명령을 사용하려면 먼저 [az login](/cli/azure/reference-index#az-login)으로 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-117">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="25687-118">로그인하면 Azure 계정에 연결된 구독 목록이 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="25687-118">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="25687-119">`isDefault: true`가 있는 구독 정보는 로그인한 후 현재 활성화된 구독입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-119">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="25687-120">다른 구독을 선택하려면 전환할 구독 ID와 함께 [az account set](/cli/azure/account#az-account-set) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-120">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="25687-121">구독 선택에 대한 자세한 내용은 [여러 Azure 구독 사용](manage-azure-subscriptions-azure-cli.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="25687-121">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="25687-122">비 대화형으로 로그인할 수 있는 방법도 여러 가지가 있으며, 이는 [Azure CLI에 로그인](authenticate-azure-cli.md)에서 자세히 설명됩니다.</span><span class="sxs-lookup"><span data-stu-id="25687-122">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="25687-123">일반적인 명령</span><span class="sxs-lookup"><span data-stu-id="25687-123">Common commands</span></span>

<span data-ttu-id="25687-124">이 표에는 CLI 및 해당 참조 설명서에 대한 링크에 사용되는 몇 가지 일반적인 명령이 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25687-124">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="25687-125">리소스 종류</span><span class="sxs-lookup"><span data-stu-id="25687-125">Resource type</span></span> | <span data-ttu-id="25687-126">Azure CLI 명령 그룹</span><span class="sxs-lookup"><span data-stu-id="25687-126">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="25687-127">리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="25687-127">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="25687-128">az group</span><span class="sxs-lookup"><span data-stu-id="25687-128">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="25687-129">가상 머신</span><span class="sxs-lookup"><span data-stu-id="25687-129">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="25687-130">az vm</span><span class="sxs-lookup"><span data-stu-id="25687-130">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="25687-131">스토리지 계정</span><span class="sxs-lookup"><span data-stu-id="25687-131">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="25687-132">az 스토리지 계정</span><span class="sxs-lookup"><span data-stu-id="25687-132">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="25687-133">Key Vault</span><span class="sxs-lookup"><span data-stu-id="25687-133">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="25687-134">az keyvault</span><span class="sxs-lookup"><span data-stu-id="25687-134">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="25687-135">웹 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="25687-135">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="25687-136">az webapp</span><span class="sxs-lookup"><span data-stu-id="25687-136">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="25687-137">SQL 데이터베이스</span><span class="sxs-lookup"><span data-stu-id="25687-137">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="25687-138">az sql server</span><span class="sxs-lookup"><span data-stu-id="25687-138">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="25687-139">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="25687-139">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="25687-140">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="25687-140">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="25687-141">명령 찾기</span><span class="sxs-lookup"><span data-stu-id="25687-141">Finding commands</span></span>

<span data-ttu-id="25687-142">CLI에서 명령은 _그룹_의 _명령_으로 조직됩니다.</span><span class="sxs-lookup"><span data-stu-id="25687-142">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="25687-143">각 그룹은 Azure 서비스를 나타내며, 명령은 해당 서비스에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-143">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="25687-144">명령을 검색하려면 [az find](/cli/azure/reference-index#az-find)를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-144">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="25687-145">예를 들어 이름에 `secret`이(가) 포함된 명령을 검색하려면 다음 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-145">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="25687-146">`--help` 인수를 사용하여 명령 및 그룹의 하위 그룹의 전체 목록을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="25687-146">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="25687-147">예를 들어, 네트워크 보안 그룹(NSG)을 사용하는 작업에 대한 CLI 명령을 찾으려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-147">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="25687-148">CLI에는 Bash 셸에서 명령에 대한 전체 탭 완성 기능이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="25687-148">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="25687-149">전역으로 사용 가능한 인수</span><span class="sxs-lookup"><span data-stu-id="25687-149">Globally available arguments</span></span>

<span data-ttu-id="25687-150">일부 인수는 모든 명령에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25687-150">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="25687-151">`--help`은(는) 명령 및 해당 인수에 대한 CLI 참조 정보를 출력하고 사용 가능한 하위 그룹 및 명령을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-151">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="25687-152">`--output`은(는) 출력 형식을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-152">`--output` changes the output format.</span></span> <span data-ttu-id="25687-153">사용 가능한 출력 형식은 `json`, `jsonc`(색이 지정된 JSON), `tsv`(탭으로 구분된 값), `table`(사람이 읽을 수 있는 ASCII 테이블) 및 `yaml`입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-153">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="25687-154">기본적인 CLI 출력은 `json`입니다.</span><span class="sxs-lookup"><span data-stu-id="25687-154">By default the CLI outputs `json`.</span></span> <span data-ttu-id="25687-155">사용 가능한 출력 형식에 대해 자세히 알아보려면 [Azure CLI의 출력 형식](format-output-azure-cli.md)을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="25687-155">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="25687-156">`--query`은(는) [JMESPath 쿼리 언어](http://jmespath.org/)를 사용하여 Azure 서비스에서 반환되는 출력을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-156">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="25687-157">쿼리에 대한 자세한 내용은 [Azure CLI를 사용한 쿼리 명령 결과](query-azure-cli.md) 및 [JMESPath 자습서](http://jmespath.org/tutorial.html)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="25687-157">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="25687-158">`--verbose`은(는) 작업 중 Azure에서 생성되는 리소스에 대한 정보 및 기타 유용한 정보를 출력합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-158">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="25687-159">`--debug`은(는) 디버깅 목적으로 사용되는 CLI 작업에 대한 자세한 정보를 출력합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-159">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="25687-160">버그가 발견된 경우, 버그 보고서를 제출할 때 `--debug` 플래그를 사용해서 생성된 출력을 제공하십시오.</span><span class="sxs-lookup"><span data-stu-id="25687-160">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="25687-161">대화형 모드</span><span class="sxs-lookup"><span data-stu-id="25687-161">Interactive mode</span></span>

<span data-ttu-id="25687-162">CLI는 도움말 정보를 자동으로 표시하고 하위 명령을 더 쉽게 선택할 수 있게 해주는 대화형 모드를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-162">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="25687-163">대화형 모드로 전환하려면 [az interactive](/cli/azure/reference-index#az-interactive) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="25687-163">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="25687-164">대화형 모드에 대한 자세한 내용은 [Azure CLI 대화형 모드](interactive-azure-cli.md)를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="25687-164">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="25687-165">또한 자동 완성 및 마우스를 위로 가져갈 때 표시되는 설명을 포함하여 대화형 환경을 제공하는 [Visual Studio Code 플러그인](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli)도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25687-165">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="25687-166">퀵 스타트 및 자습서로 CLI 기본 내용 학습</span><span class="sxs-lookup"><span data-stu-id="25687-166">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="25687-167">Azure CLI를 시작하려면 가상 머신 설정 및 Azure 리소스 쿼리를 위한 CLI 기능 사용에 대한 세부 자습서를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="25687-167">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="25687-168">Azure CLI를 사용하여 가상 머신 만들기 자습서</span><span class="sxs-lookup"><span data-stu-id="25687-168">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="25687-169">다른 인기 있는 서비스에 대한 빠른 시작도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25687-169">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="25687-170">Azure CLI를 사용하여 스토리지 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="25687-170">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="25687-171">CLI를 사용하여 Azure Blob Storage에 대한 개체 전송</span><span class="sxs-lookup"><span data-stu-id="25687-171">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="25687-172">Azure CLI를 사용하여 단일 Azure SQL 데이터베이스 만들기</span><span class="sxs-lookup"><span data-stu-id="25687-172">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="25687-173">Azure CLI를 사용하여 Azure Database for MySQL 서버 만들기</span><span class="sxs-lookup"><span data-stu-id="25687-173">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="25687-174">Azure CLI를 사용하여 PostgreSQL용 Azure Database 만들기</span><span class="sxs-lookup"><span data-stu-id="25687-174">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="25687-175">Azure에서 Python 웹앱 만들기</span><span class="sxs-lookup"><span data-stu-id="25687-175">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="25687-176">Azure Web Apps for Containers에서 사용자 지정 Docker Hub 이미지 실행</span><span class="sxs-lookup"><span data-stu-id="25687-176">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="25687-177">피드백 제공</span><span class="sxs-lookup"><span data-stu-id="25687-177">Give feedback</span></span>

<span data-ttu-id="25687-178">CLI 기능 개선 및 버그 해결을 위해 피드백을 보내주시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="25687-178">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="25687-179">[GitHub에서 문제를 제출](https://github.com/azure/azure-cli/issues)하거나 CLI의 기본 제공 기능을 사용하여 [az feedback](/cli/azure/reference-index#az-feedback) 명령을 통해 일반적인 피드백을 남길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25687-179">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

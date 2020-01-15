---
title: Azure CLI 별칭 확장
description: Azure CLI 별칭 확장 사용 방법
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cc6192c3e78f7bc895ed8f4c2f640aa1bf0e883c
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913674"
---
# <a name="the-azure-cli-alias-extension"></a><span data-ttu-id="d0db3-103">Azure CLI 별칭 확장</span><span class="sxs-lookup"><span data-stu-id="d0db3-103">The Azure CLI alias extension</span></span>

<span data-ttu-id="d0db3-104">별칭 확장을 사용하면 기존 명령을 사용하여 Azure CLI에 대한 사용자 정의 명령을 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="d0db3-105">별칭은 바로 가기를 허용하여 워크플로 단순하게 유지하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-105">Aliases help keep your workflow simple by allowing shortcuts.</span></span> <span data-ttu-id="d0db3-106">별칭은 Jinja2 템플릿 엔진을 기반으로 하기 때문에 고급 인수 처리도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="d0db3-107">별칭 확장은 공개 미리 보기에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="d0db3-108">기능 및 구성 파일 형식이 변경될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="d0db3-109">별칭 확장 설치</span><span class="sxs-lookup"><span data-stu-id="d0db3-109">Install the alias extension</span></span>

<span data-ttu-id="d0db3-110">별칭 확장을 사용하는 데 필요한 최소 Azure CLI 버전은 **2.0.28**입니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="d0db3-111">CLI 버전을 확인하려면 `az --version`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="d0db3-112">설치를 업데이트해야 하는 경우 [Azure CLI 설치](./install-azure-cli.md)의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI](./install-azure-cli.md).</span></span>

<span data-ttu-id="d0db3-113">[az extension add](/cli/azure/extension#az-extension-add) 명령을 사용하여 확장을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="d0db3-114">[az 확장 목록](/cli/azure/extension#az-extension-list)을 사용하여 확장 설치를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="d0db3-115">별칭 확장이 제대로 설치된 경우 명령 출력에 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="d0db3-116">확장을 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="d0db3-116">Keep the extension up-to-date</span></span>

<span data-ttu-id="d0db3-117">별칭 확장은 현재 개발 중이며 새 버전은 정기적으로 릴리스됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="d0db3-118">CLI를 업데이트하는 경우 새 버전이 설치되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-118">New versions aren't installed when you update the CLI.</span></span> <span data-ttu-id="d0db3-119">[az 확장 업데이트](/cli/azure/extension#az-extension-update)를 사용하여 확장 업데이트를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="d0db3-120">Azure CLI에 대한 별칭 관리</span><span class="sxs-lookup"><span data-stu-id="d0db3-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="d0db3-121">별칭 확장을 사용하여 다른 CLI 명령에 대한 별칭을 만들고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-121">The alias extension lets you create and manage aliases for other CLI commands.</span></span> <span data-ttu-id="d0db3-122">모든 사용 가능한 명령 및 매개 변수 세부 정보를 보려면 `--help`을 사용하여 별칭 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-122">To view all the available commands and parameter details, run the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="d0db3-123">간단한 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="d0db3-123">Create simple alias commands</span></span>

<span data-ttu-id="d0db3-124">별칭을 사용하면 기존 명령 그룹이나 명령 이름을 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="d0db3-125">예를 들어 `group` 명령 그룹을 `rg`로, `list` 명령을 `ls`로 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="d0db3-126">이렇게 새로 정의된 별칭은 정의가 될 수 있는 어느 곳에서든 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="d0db3-127">`az`이 명령의 일부로 포함되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="d0db3-128">별칭은 전체 명령의 바로 가기일 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="d0db3-129">다음 예는 사용 가능한 리소스 그룹과 해당 위치를 테이블로 출력하여 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="d0db3-130">이제 `ls-groups`는 다른 CLI 명령처럼 실행될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="d0db3-131">인수를 사용하여 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="d0db3-131">Create an alias command with arguments</span></span>

<span data-ttu-id="d0db3-132">별칭 이름에 위치 인수를 `{{ arg_name }}`으로 포함하여 별칭 명령에 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="d0db3-133">중괄호 안의 공백이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="d0db3-134">다음 예제 별칭은 위치 인수를 사용하여 VM의 공용 IP 주소를 얻는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="d0db3-135">이 명령을 실행할 때 위치 인수에 값을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="d0db3-136">별칭 명령에서 환경 변수를 사용할 수도 있으며, 이 명령은 런타임에서 평가됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-136">You can also use environment variables in aliased commands, which are evaluated at runtime.</span></span> <span data-ttu-id="d0db3-137">다음 예는 `eastus`에 리소스 그룹을 만들고 `owner` 태그를 추가하는 `create-rg` 별칭을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="d0db3-138">이 태그에는 로컬 환경 변수 `USER`의 값이 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="d0db3-139">별칭의 명령 내부 환경 변수를 등록하려면 달러 기호 `$`이 이스케이프 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="d0db3-140">Jinja2 템플릿을 사용하는 프로세스 인수</span><span class="sxs-lookup"><span data-stu-id="d0db3-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="d0db3-141">[Jinja2](http://jinja.pocoo.org/docs/2.10/)로 별칭 확장에서 인수 대체를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span></span> <span data-ttu-id="d0db3-142">Jinja2 템플릿은 인수 조작을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-142">Jinja2 templates allow for manipulating the arguments.</span></span>

<span data-ttu-id="d0db3-143">Jinja2 템플릿을 사용하면 기본 명령과 다른 인수 유형을 사용하는 별칭을 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-143">With Jinja2 templates, you can write aliases that take different types of arguments than the underlying command.</span></span> <span data-ttu-id="d0db3-144">예를 들어 스토리지 URL을 사용하는 별칭을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-144">For example, you can make an alias that takes a storage URL.</span></span> <span data-ttu-id="d0db3-145">그런 다음 이 URL을 구문 분석하여 계정 및 컨테이너 이름을 스토리지 명령에 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="d0db3-146">Jinja2 템플릿 엔진에 대한 자세한 내용은 [Jinja2 설명서](http://jinja.pocoo.org/docs/2.10/templates/)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0db3-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="d0db3-147">별칭 구성 파일</span><span class="sxs-lookup"><span data-stu-id="d0db3-147">Alias configuration file</span></span>

<span data-ttu-id="d0db3-148">별칭을 만들고 수정하는 또 다른 방법은 별칭 구성 파일을 변경하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="d0db3-149">별칭 명령 정의는 `$AZURE_USER_CONFIG/alias`에있는 구성 파일에 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="d0db3-150">`AZURE_USER_CONFIG`의 기본값은 macOS와 Linux의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="d0db3-151">별칭 구성 파일은 INI 구성 파일 형식으로 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="d0db3-152">별칭 명령의 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="d0db3-153">위치 인수가 있는 별칭의 경우, 별칭 명령에 대한 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-153">For aliases that have positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="d0db3-154">별칭 구성 파일을 통해 인수를 갖는 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="d0db3-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="d0db3-155">다음 예제에서는 인수를 사용하는 명령에 대한 별칭을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-155">The next example shows an alias for a command with arguments.</span></span> <span data-ttu-id="d0db3-156">이 명령은 VM에 대한 공용 IP 주소를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-156">This command gets the public IP address for a VM.</span></span> <span data-ttu-id="d0db3-157">별칭이 지정된 명령은 단일 줄에 있어야 하며, 별칭 이름에 모든 인수를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-157">Aliased commands must all be on a single line, and use all of the arguments in the alias name.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="d0db3-158">별칭 확장 제거</span><span class="sxs-lookup"><span data-stu-id="d0db3-158">Uninstall the alias extension</span></span>

<span data-ttu-id="d0db3-159">확장을 설치 제거하려면 [az extension remove](/cli/azure/extension#az-extension-remove) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-159">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="d0db3-160">확장 관련 버그 또는 기타 문제로 인해 제거한 경우 [GitHub 문제를 제출](https://github.com/Azure/azure-cli-extensions/issues)하면 수정 사항을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0db3-160">If you uninstalled because a bug or other problem with the extension, [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>

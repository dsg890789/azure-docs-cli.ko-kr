---
title: Azure CLI 2.0 별칭 확장
description: Azure CLI 2.0 별칭 확장 사용 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d6eae7f5a6ca30af7214e77ae561c3a53a2cee26
ms.sourcegitcommit: 204fd027d3668959b98b936969ccb41eada0fd29
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/16/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="69278-103">Azure CLI 2.0 별칭 확장</span><span class="sxs-lookup"><span data-stu-id="69278-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="69278-104">별칭 확장을 사용하면 기존 명령을 사용하여 Azure CLI에 대한 사용자 정의 명령을 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="69278-105">별칭을 사용하면 바로 가기를 허용하고 위치 인수를 사용할 수 있으므로 워크플로를 간결하고 간단하게 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="69278-106">별칭은 Jinja2 템플릿 엔진을 기반으로 하기 때문에 고급 인수 처리도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="69278-107">별칭 확장은 공개 미리 보기에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="69278-108">기능 및 구성 파일 형식이 변경될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="69278-109">별칭 확장 설치</span><span class="sxs-lookup"><span data-stu-id="69278-109">Install the alias extension</span></span>

<span data-ttu-id="69278-110">별칭 확장을 사용하는 데 필요한 최소 Azure CLI 버전은 **2.0.28**입니다.</span><span class="sxs-lookup"><span data-stu-id="69278-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="69278-111">CLI 버전을 확인하려면 `az --version`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="69278-112">설치를 업데이트해야 하는 경우 [Azure CLI 2.0 설치](./install-azure-cli.md)의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="69278-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="69278-113">[az extension add](/cli/azure/extension#az-extension-add) 명령을 사용하여 확장을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="69278-114">[az 확장 목록](/cli/azure/extension#az-extension-list)을 사용하여 확장 설치를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="69278-115">별칭 확장이 제대로 설치된 경우 명령 출력에 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```


## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="69278-116">확장을 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="69278-116">Keep the extension up to date</span></span>

<span data-ttu-id="69278-117">별칭 확장은 현재 개발 중이며 새 버전은 정기적으로 릴리스됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="69278-118">새 버전은 CLI를 업데이트할 때마다 자동으로 설치되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="69278-119">[az 확장 업데이트](/cli/azure/extension#az-extension-update)를 사용하여 확장 업데이트를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```


## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="69278-120">Azure CLI에 대한 별칭 관리</span><span class="sxs-lookup"><span data-stu-id="69278-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="69278-121">별칭 확장은 별칭을 관리하는데 편리하고 친숙한 명령을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-121">The alias extension provides convenient and familiar commands to manage aliases.</span></span> <span data-ttu-id="69278-122">모든 사용 가능한 명령 및 매개 변수 세부 정보를 보려면 `--help`을 사용하여 별칭 명령을 호출합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-122">To view all the available commands and parameter details, invoke the alias command with `--help`.</span></span>

```azurecli
az alias --help
```


## <a name="create-simple-alias-commands"></a><span data-ttu-id="69278-123">간단한 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="69278-123">Create simple alias commands</span></span>

<span data-ttu-id="69278-124">별칭을 사용하면 기존 명령 그룹이나 명령 이름을 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="69278-125">예를 들어 `group` 명령 그룹을 `rg`로, `list` 명령을 `ls`로 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="69278-126">이렇게 새로 정의된 별칭은 정의가 될 수 있는 어느 곳에서든 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="69278-127">`az`이 명령의 일부로 포함되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="69278-128">별칭은 전체 명령의 바로 가기일 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="69278-129">다음 예는 사용 가능한 리소스 그룹과 해당 위치를 테이블로 출력하여 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="69278-130">이제 `ls-groups`는 다른 CLI 명령처럼 실행될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```


## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="69278-131">인수를 사용하여 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="69278-131">Create an alias command with arguments</span></span>

<span data-ttu-id="69278-132">별칭 이름에 위치 인수를 `{{ arg_name }}`으로 포함하여 별칭 명령에 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="69278-133">중괄호 안의 공백이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-133">The whitespace inside the braces is required.</span></span>

```azurecli
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="69278-134">다음 예제 별칭은 위치 인수를 사용하여 VM의 공용 IP 주소를 얻는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="69278-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="69278-135">이 명령을 실행할 때 위치 인수에 값을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="69278-136">별칭으로 호출된 명령에서 환경 변수를 사용할 수도 있으며, 이 명령은 런타임에서 평가됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-136">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="69278-137">다음 예는 `eastus`에 리소스 그룹을 만들고 `owner` 태그를 추가하는 `create-rg` 별칭을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="69278-138">이 태그에는 로컬 환경 변수 `USER`의 값이 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="69278-139">별칭의 명령 내부 환경 변수를 등록하려면 달러 기호 `$`이 이스케이프 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>


## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="69278-140">Jinja2 템플릿을 사용하는 프로세스 인수</span><span class="sxs-lookup"><span data-stu-id="69278-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="69278-141">별칭 확장의 인수 대체는 [Jinja2](http://jinja.pocoo.org/docs/2.10/)에 의해 수행되어 Jinja2 템플릿 엔진의 기능에 대한 모든 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="69278-142">템플릿을 사용하면 문자열에서 데이터 추출 및 대체와 같은 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-142">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="69278-143">Jinja2 템플릿을 사용하면 기본 명령과 다른 인수 유형을 사용하는 별칭을 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-143">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="69278-144">예를 들어 저장소 URL을 사용하는 별칭을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-144">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="69278-145">그런 다음 이 URL을 구문 분석하여 계정 및 컨테이너 이름을 저장소 명령에 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="69278-146">Jinja2 템플릿 엔진에 대한 자세한 내용은 [Jinja2 설명서](http://jinja.pocoo.org/docs/2.10/templates/)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="69278-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>


## <a name="alias-configuration-file"></a><span data-ttu-id="69278-147">별칭 구성 파일</span><span class="sxs-lookup"><span data-stu-id="69278-147">Alias configuration file</span></span>

<span data-ttu-id="69278-148">별칭을 만들고 수정하는 또 다른 방법은 별칭 구성 파일을 변경하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="69278-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="69278-149">별칭 명령 정의는 `$AZURE_USER_CONFIG/alias`에있는 구성 파일에 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="69278-150">`AZURE_USER_CONFIG`의 기본값은 macOS와 Linux의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다.</span><span class="sxs-lookup"><span data-stu-id="69278-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="69278-151">별칭 구성 파일은 INI 구성 파일 형식으로 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="69278-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="69278-152">별칭 명령의 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="69278-153">위치 인수가 포함된 별칭의 경우, 별칭 명령에 대한 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-153">For aliases that contain positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```


## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="69278-154">별칭 구성 파일을 통해 인수를 갖는 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="69278-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="69278-155">다음은 VM의 공용 IP 주소를 가져오는 인수가 있는 예제 별칭 명령을 포함하는 별칭 구성 파일입니다.</span><span class="sxs-lookup"><span data-stu-id="69278-155">Below is an alias configuration file that contains an example alias command with arguments, which gets the public IP address for a VM.</span></span> <span data-ttu-id="69278-156">호출된 명령이 한 줄에 있으며 별칭에 정의된 동일한 인수를 포함하는지 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="69278-156">Ensure that the invoked command is in a single line, and contains the same arguments defined in the alias.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```


## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="69278-157">별칭 확장 제거</span><span class="sxs-lookup"><span data-stu-id="69278-157">Uninstall the alias extension</span></span>

<span data-ttu-id="69278-158">확장을 설치 제거하려면 [az extension remove](/cli/azure/extension#az-extension-remove) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="69278-158">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli
az extension remove --name alias
```

<span data-ttu-id="69278-159">확장 관련 버그 또는 기타 문제로 인해 제거한 경우 [GitHub 문제를 제출](https://github.com/Azure/azure-cli-extensions/issues)하면 수정 사항을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69278-159">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>

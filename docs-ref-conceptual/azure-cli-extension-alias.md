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
ms.openlocfilehash: e457d78b1009fe573554df36db18f525516e0b4a
ms.sourcegitcommit: 335c11e6c34f7907e61a43507745ba84ed4e7469
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="54113-103">Azure CLI 2.0 별칭 확장</span><span class="sxs-lookup"><span data-stu-id="54113-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="54113-104">별칭 확장을 사용하면 기존 명령을 사용하여 Azure CLI에 대한 사용자 정의 명령을 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="54113-105">별칭을 사용하면 바로 가기를 허용하고 위치 인수를 사용할 수 있으므로 워크플로를 간결하고 간단하게 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="54113-106">별칭은 Jinja2 템플릿 엔진을 기반으로 하기 때문에 고급 인수 처리도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="54113-107">별칭 확장은 공개 미리 보기에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="54113-108">기능 및 구성 파일 형식이 변경될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="54113-109">별칭 확장 설치</span><span class="sxs-lookup"><span data-stu-id="54113-109">Install the alias extension</span></span>

<span data-ttu-id="54113-110">별칭 확장을 사용하는 데 필요한 최소 Azure CLI 버전은 **2.0.28**입니다.</span><span class="sxs-lookup"><span data-stu-id="54113-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="54113-111">CLI 버전을 확인하려면 `az --version`을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="54113-112">설치를 업데이트해야 하는 경우 [Azure CLI 2.0 설치](./install-azure-cli.md)의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="54113-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="54113-113">[az extension add](/cli/azure/extension#az-extension-add) 명령을 사용하여 확장을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="54113-114">[az 확장 목록](/cli/azure/extension#az-extension-list)을 사용하여 확장 설치를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="54113-115">별칭 확장이 제대로 설치된 경우 명령 출력에 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="54113-116">확장을 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="54113-116">Keep the extension up to date</span></span>

<span data-ttu-id="54113-117">별칭 확장은 현재 개발 중이며 새 버전은 정기적으로 릴리스됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="54113-118">새 버전은 CLI를 업데이트할 때마다 자동으로 설치되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="54113-119">[az 확장 업데이트](/cli/azure/extension#az-extension-update)를 사용하여 확장 업데이트를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a><span data-ttu-id="54113-120">별칭 명령 파일 형식</span><span class="sxs-lookup"><span data-stu-id="54113-120">Alias commands file format</span></span>

<span data-ttu-id="54113-121">별칭 명령 정의는 `$AZURE_USER_CONFIG/alias`에있는 구성 파일에 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-121">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="54113-122">`AZURE_USER_CONFIG`의 기본값은 macOS와 Linux의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다.</span><span class="sxs-lookup"><span data-stu-id="54113-122">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="54113-123">별칭 구성 파일은 INI 구성 파일 형식으로 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-123">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="54113-124">별칭 명령의 일반적인 형식은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-124">The general format for alias commands is:</span></span>

```
[command_name]
command = invoked_commands
```

<span data-ttu-id="54113-125">명령의 일부로 `az`를 포함하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="54113-125">Don't include `az` as part of the command.</span></span>

## <a name="create-simple-alias-commands"></a><span data-ttu-id="54113-126">간단한 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="54113-126">Create simple alias commands</span></span>

<span data-ttu-id="54113-127">별칭을 사용하면 기존 명령 그룹이나 명령 이름을 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-127">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="54113-128">예를 들어 `group` 명령 그룹을 `rg`로, `list` 명령을 `ls`로 단축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-128">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```
[rg]
command = group

[ls]
command = list
```

<span data-ttu-id="54113-129">이렇게 새로 정의된 별칭은 정의가 될 수 있는 어느 곳에서든 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-129">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="54113-130">별칭은 전체 명령의 바로 가기일 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-130">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="54113-131">다음 예는 사용 가능한 리소스 그룹과 해당 위치를 테이블로 출력하여 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-131">The next example lists available resource groups and their locations in table output:</span></span>

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

<span data-ttu-id="54113-132">이제 `ls-groups`는 다른 CLI 명령처럼 실행될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-132">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="54113-133">인수를 사용하여 별칭 명령 만들기</span><span class="sxs-lookup"><span data-stu-id="54113-133">Create an alias command with arguments</span></span>

<span data-ttu-id="54113-134">별칭 이름에 위치 인수를 `{{ arg_name }}`으로 포함하여 별칭 명령에 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-134">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="54113-135">중괄호 안의 공백이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-135">The whitespace inside the braces is required.</span></span>

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

<span data-ttu-id="54113-136">다음 예제 별칭은 위치 인수를 사용하여 VM의 공용 IP 주소를 얻는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="54113-136">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

<span data-ttu-id="54113-137">이 명령을 실행할 때 위치 인수에 값을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-137">When running this command, you give values to the positional arguments.</span></span>

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="54113-138">별칭으로 호출된 명령에서 환경 변수를 사용할 수도 있으며, 이 명령은 런타임에서 평가됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-138">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="54113-139">다음 예는 `eastus`에 리소스 그룹을 만들고 `owner` 태그를 추가하는 `create-rg` 별칭을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-139">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="54113-140">이 태그에는 로컬 환경 변수 `USER`의 값이 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="54113-140">This tag is assigned the value of the local environment variable `USER`.</span></span>

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="54113-141">Jinja2 템플릿을 사용하는 프로세스 인수</span><span class="sxs-lookup"><span data-stu-id="54113-141">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="54113-142">별칭 확장의 인수 대체는 [Jinja2](http://jinja.pocoo.org/docs/2.10/)에 의해 수행되어 Jinja2 템플릿 엔진의 기능에 대한 모든 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-142">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="54113-143">템플릿을 사용하면 문자열에서 데이터 추출 및 대체와 같은 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-143">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="54113-144">Jinja2 템플릿을 사용하면 기본 명령과 다른 인수 유형을 사용하는 별칭을 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-144">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="54113-145">예를 들어 저장소 URL을 사용하는 별칭을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-145">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="54113-146">그런 다음 이 URL을 구문 분석하여 계정 및 컨테이너 이름을 저장소 명령에 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-146">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

<span data-ttu-id="54113-147">Jinja2 템플릿 엔진에 대한 자세한 내용은 [Jinja2 설명서](http://jinja.pocoo.org/docs/2.10/templates/)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="54113-147">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="54113-148">별칭 확장 제거</span><span class="sxs-lookup"><span data-stu-id="54113-148">Uninstall the alias extension</span></span>

<span data-ttu-id="54113-149">확장을 설치 제거하려면 [az extension remove](/cli/azure/extension#az-extension-remove) 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="54113-149">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli
az extension remove --name alias
```

<span data-ttu-id="54113-150">확장 관련 버그 또는 기타 문제로 인해 제거한 경우 [GitHub 문제를 제출](https://github.com/Azure/azure-cli-extensions/issues)하면 수정 사항을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54113-150">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>

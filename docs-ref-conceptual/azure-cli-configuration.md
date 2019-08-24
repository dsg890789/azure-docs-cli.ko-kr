---
title: Azure CLI 구성 옵션
description: Azure CLI 구성 방법
keywords: Azure CLI, 구성, 설정, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d23f576a1f7447ffab0606b4554a81ae5c536e85
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158491"
---
# <a name="azure-cli-configuration"></a><span data-ttu-id="d0443-104">Azure CLI 구성</span><span class="sxs-lookup"><span data-stu-id="d0443-104">Azure CLI configuration</span></span>

<span data-ttu-id="d0443-105">Azure CLI는 로깅, 데이터 컬렉션 및 기본 인수 값과 같은 사용자 구성 설정을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-105">The Azure CLI allows for user configuration for settings such as logging, data collection, and default argument values.</span></span>
<span data-ttu-id="d0443-106">CLI는 몇 가지 기본값을 관리하기 위한 편리한 명령 `az configure`를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-106">The CLI offers a convenience command for managing some defaults, `az configure`.</span></span> <span data-ttu-id="d0443-107">구성 파일 또는 환경 변수를 사용하여 다른 값을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-107">Other values can be set in a configuration file or with environment variables.</span></span>

<span data-ttu-id="d0443-108">CLI에서 사용되는 구성 값은 다음 우선 순위에서 평가되며 목록의 상위 항목이 우선 순위를 갖습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-108">Configuration values used by the CLI are evaluated in the following precedence, with items higher on the list taking priority.</span></span>

1. <span data-ttu-id="d0443-109">명령줄 매개 변수</span><span class="sxs-lookup"><span data-stu-id="d0443-109">Command-line parameters</span></span>
2. <span data-ttu-id="d0443-110">환경 변수</span><span class="sxs-lookup"><span data-stu-id="d0443-110">Environment variables</span></span>
3. <span data-ttu-id="d0443-111">구성 파일의 값 또는 `az configure`로 사용</span><span class="sxs-lookup"><span data-stu-id="d0443-111">Values in the configuration file or set with `az configure`</span></span>

## <a name="cli-configuration-with-az-configure"></a><span data-ttu-id="d0443-112">az configure으로 CLI 구성</span><span class="sxs-lookup"><span data-stu-id="d0443-112">CLI configuration with az configure</span></span>

<span data-ttu-id="d0443-113">[az configure](/cli/azure/reference-index#az-configure) 명령으로 CLI에 대한 기본값을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-113">You set defaults for the CLI with the [az configure](/cli/azure/reference-index#az-configure) command.</span></span>
<span data-ttu-id="d0443-114">이 명령은 하나의 인수인 `--defaults`를 취하며 공백으로 구분된 `key=value` 쌍의 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-114">This command takes one argument, `--defaults`, which is a space-separated list of `key=value` pairs.</span></span> <span data-ttu-id="d0443-115">제공된 값은 CLI에서 필수 인수 대신 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-115">The provided values are used by the CLI in place of required arguments.</span></span>

<span data-ttu-id="d0443-116">다음 표는 사용할 수 있는 구성 키의 목록을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-116">The following table contains a list of available configuration keys.</span></span>

| <span data-ttu-id="d0443-117">Name</span><span class="sxs-lookup"><span data-stu-id="d0443-117">Name</span></span> | <span data-ttu-id="d0443-118">설명</span><span class="sxs-lookup"><span data-stu-id="d0443-118">Description</span></span> |
|------|-------------|
| <span data-ttu-id="d0443-119">group</span><span class="sxs-lookup"><span data-stu-id="d0443-119">group</span></span> | <span data-ttu-id="d0443-120">모든 명령에 사용할 기본 리소스 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-120">The default resource group to use for all commands.</span></span> |
| <span data-ttu-id="d0443-121">location</span><span class="sxs-lookup"><span data-stu-id="d0443-121">location</span></span> | <span data-ttu-id="d0443-122">모든 명령에 사용할 기본 위치입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-122">The default location to use for all commands.</span></span> |
| <span data-ttu-id="d0443-123">web</span><span class="sxs-lookup"><span data-stu-id="d0443-123">web</span></span> | <span data-ttu-id="d0443-124">`az webapp` 명령에 사용할 기본 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-124">The default app name to use for `az webapp` commands.</span></span> |
| <span data-ttu-id="d0443-125">vm</span><span class="sxs-lookup"><span data-stu-id="d0443-125">vm</span></span> | <span data-ttu-id="d0443-126">`az vm` 명령에 사용할 기본 VM 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-126">The default VM name to use for `az vm` commands.</span></span> |
| <span data-ttu-id="d0443-127">vmss</span><span class="sxs-lookup"><span data-stu-id="d0443-127">vmss</span></span> | <span data-ttu-id="d0443-128">`az vmss` 명령에 사용할 기본 가상 머신 확장 집합(VMSS) 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-128">The default virtual machine scale set (VMSS) name to use for  `az vmss` commands.</span></span> |
| <span data-ttu-id="d0443-129">acr</span><span class="sxs-lookup"><span data-stu-id="d0443-129">acr</span></span> | <span data-ttu-id="d0443-130">`az acr` 명령에 사용할 기본 컨테이너 레지스트리 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-130">The default container registry name to use for `az acr` commands.</span></span> |

<span data-ttu-id="d0443-131">예를 들어, 다음은 모든 명령에 대해 기본 리소스 그룹 및 위치를 설정하는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-131">As an example, here's how you would set the default resource group and location for all commands.</span></span>

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a><span data-ttu-id="d0443-132">CLI 구성 파일</span><span class="sxs-lookup"><span data-stu-id="d0443-132">CLI configuration file</span></span>

<span data-ttu-id="d0443-133">CLI 구성 파일에는 CLI 동작 관리에 사용되는 다른 설정이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-133">The CLI configuration file contains other settings that are used for managing CLI behavior.</span></span> <span data-ttu-id="d0443-134">구성 파일 자체는 `$AZURE_CONFIG_DIR/config`에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-134">The configuration file itself is located at `$AZURE_CONFIG_DIR/config`.</span></span> <span data-ttu-id="d0443-135">`AZURE_CONFIG_DIR`의 기본값은 Linux와 macOS의 경우 `$HOME/.azure`이고 Windows의 경우 `%USERPROFILE%\.azure`입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-135">The default value of `AZURE_CONFIG_DIR` is `$HOME/.azure` on Linux and macOS, and `%USERPROFILE%\.azure` on Windows.</span></span>

<span data-ttu-id="d0443-136">구성 파일은 INI 파일 형식으로 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-136">Configuration files are written in the INI file format.</span></span> <span data-ttu-id="d0443-137">이 파일 형식은 섹션 헤더, 그리고 키-값 항목 목록에 의해 정의됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-137">This file format is defined by section headers, followed by a list of key-value entries.</span></span>

* <span data-ttu-id="d0443-138">섹션 헤더는 `[section-name]`으로 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-138">Section headers are written as `[section-name]`.</span></span> <span data-ttu-id="d0443-139">섹션 이름은 대/소문자를 구분합니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-139">Section names are case-sensitive.</span></span>
* <span data-ttu-id="d0443-140">항목은 `key=value`로 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-140">Entries are written as `key=value`.</span></span> <span data-ttu-id="d0443-141">키 이름은 대/소문자를 구분하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-141">Key names are not case-sensitive.</span></span>
* <span data-ttu-id="d0443-142">설명은 `#` 또는 `;`으로 시작하는 줄입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-142">Comments are any line that begins with a `#` or `;`.</span></span> <span data-ttu-id="d0443-143">인라인 주석은 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-143">Inline comments are not allowed.</span></span>

<span data-ttu-id="d0443-144">부울은 대/소문자를 구분하며 다음 값으로 표현됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-144">Booleans are case-insensitive, and are represented by the following values.</span></span>

* <span data-ttu-id="d0443-145">__참__: 1, yes, true, on</span><span class="sxs-lookup"><span data-stu-id="d0443-145">__True__: 1, yes, true, on</span></span>
* <span data-ttu-id="d0443-146">__거짓__: 0, no, false, off</span><span class="sxs-lookup"><span data-stu-id="d0443-146">__False__: 0, no, false, off</span></span>

<span data-ttu-id="d0443-147">다음은 확인 프롬프트를 비활성화하고 `/var/log/azure` 디렉토리에 로깅을 설정하는 CLI 구성 파일의 예입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-147">Here's an example of a CLI configuration file that disables any confirmation prompts and sets up logging to the `/var/log/azure` directory.</span></span>

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

<span data-ttu-id="d0443-148">모든 사용 가능한 구성 값과 그 의미에 대한 자세한 내용은 다음 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0443-148">See the next section for details on all of the available configuration values and what they mean.</span></span> <span data-ttu-id="d0443-149">INI 파일 형식에 전체 세부 정보는 [INI에 대한 Python 문서](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0443-149">For the full details on the INI file format, see the [Python documentation on INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).</span></span>

## <a name="cli-configuration-values-and-environment-variables"></a><span data-ttu-id="d0443-150">CLI 구성 값 및 환경 변수</span><span class="sxs-lookup"><span data-stu-id="d0443-150">CLI configuration values and environment variables</span></span>

<span data-ttu-id="d0443-151">다음 표에는 구성 파일에 배치할 수 있는 모든 섹션 및 옵션 이름이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-151">The following table contains all of the sections and option names that can be placed in a configuration file.</span></span> <span data-ttu-id="d0443-152">해당 환경 변수는 모두 대문자로 `AZURE_{section}_{name}`으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-152">Their corresponding environment variables are set as `AZURE_{section}_{name}`, in all caps.</span></span> <span data-ttu-id="d0443-153">예를 들어, `batchai`에 대한 `storage_account` 기본값은 `AZURE_BATCHAI_STORAGE_ACCOUNT` 변수에 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-153">For example, the `storage_account` default for `batchai` is set in the `AZURE_BATCHAI_STORAGE_ACCOUNT` variable.</span></span>

<span data-ttu-id="d0443-154">기본값을 제공하면, 명령에 더 이상 인수가 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-154">When you provide a default value, that argument is no longer required by any command.</span></span> <span data-ttu-id="d0443-155">대신 기본값이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-155">Instead, the default value is used.</span></span>

| <span data-ttu-id="d0443-156">섹션</span><span class="sxs-lookup"><span data-stu-id="d0443-156">Section</span></span> | <span data-ttu-id="d0443-157">Name</span><span class="sxs-lookup"><span data-stu-id="d0443-157">Name</span></span>      | <span data-ttu-id="d0443-158">Type</span><span class="sxs-lookup"><span data-stu-id="d0443-158">Type</span></span> | <span data-ttu-id="d0443-159">설명</span><span class="sxs-lookup"><span data-stu-id="d0443-159">Description</span></span>|
|---------|-----------|------|------------|
| <span data-ttu-id="d0443-160">__core__</span><span class="sxs-lookup"><span data-stu-id="d0443-160">__core__</span></span> | <span data-ttu-id="d0443-161">output</span><span class="sxs-lookup"><span data-stu-id="d0443-161">output</span></span> | <span data-ttu-id="d0443-162">string</span><span class="sxs-lookup"><span data-stu-id="d0443-162">string</span></span> | <span data-ttu-id="d0443-163">기본 출력 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-163">The default output format.</span></span> <span data-ttu-id="d0443-164">`json`, `jsonc`, `tsv` 또는 `table` 중 하나일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-164">Can be one of `json`, `jsonc`, `tsv`, or `table`.</span></span> |
| | <span data-ttu-id="d0443-165">disable\_confirm\_prompt</span><span class="sxs-lookup"><span data-stu-id="d0443-165">disable\_confirm\_prompt</span></span> | <span data-ttu-id="d0443-166">부울</span><span class="sxs-lookup"><span data-stu-id="d0443-166">boolean</span></span> | <span data-ttu-id="d0443-167">확인 메시지를 표시하거나 표시하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-167">Turn confirmation prompts on/off.</span></span> |
| | <span data-ttu-id="d0443-168">collect\_telemetry</span><span class="sxs-lookup"><span data-stu-id="d0443-168">collect\_telemetry</span></span> | <span data-ttu-id="d0443-169">부울</span><span class="sxs-lookup"><span data-stu-id="d0443-169">boolean</span></span> | <span data-ttu-id="d0443-170">Microsoft가 CLI의 사용에 대해 익명의 데이터를 수집하도록 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-170">Allow Microsoft to collect anonymous data on the usage of the CLI.</span></span> <span data-ttu-id="d0443-171">개인 정보에 대한 자세한 내용은 [Azure CLI 사용 약관](http://aka.ms/AzureCliLegal)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0443-171">For privacy information, see the [Azure CLI Terms of Use](http://aka.ms/AzureCliLegal).</span></span> |
| <span data-ttu-id="d0443-172">__logging__</span><span class="sxs-lookup"><span data-stu-id="d0443-172">__logging__</span></span> | <span data-ttu-id="d0443-173">enable\_log\_file</span><span class="sxs-lookup"><span data-stu-id="d0443-173">enable\_log\_file</span></span> | <span data-ttu-id="d0443-174">부울</span><span class="sxs-lookup"><span data-stu-id="d0443-174">boolean</span></span> | <span data-ttu-id="d0443-175">로깅을 켜거나 끕니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-175">Turn logging on/off.</span></span> |
| | <span data-ttu-id="d0443-176">log\_dir</span><span class="sxs-lookup"><span data-stu-id="d0443-176">log\_dir</span></span> | <span data-ttu-id="d0443-177">string</span><span class="sxs-lookup"><span data-stu-id="d0443-177">string</span></span> | <span data-ttu-id="d0443-178">로그를 쓸 디렉터리입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-178">The directory to write logs to.</span></span> <span data-ttu-id="d0443-179">이 값은 기본적으로 `${AZURE_CONFIG_DIR}/logs`입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-179">By default this value is `${AZURE_CONFIG_DIR}/logs`.</span></span> |
| <span data-ttu-id="d0443-180">__storage__</span><span class="sxs-lookup"><span data-stu-id="d0443-180">__storage__</span></span> | <span data-ttu-id="d0443-181">connection\_string</span><span class="sxs-lookup"><span data-stu-id="d0443-181">connection\_string</span></span> | <span data-ttu-id="d0443-182">string</span><span class="sxs-lookup"><span data-stu-id="d0443-182">string</span></span> | <span data-ttu-id="d0443-183">`az storage` 명령에 사용할 기본 연결 문자열입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-183">The default connection string to use for `az storage` commands.</span></span> |
| | <span data-ttu-id="d0443-184">계정</span><span class="sxs-lookup"><span data-stu-id="d0443-184">account</span></span> | <span data-ttu-id="d0443-185">string</span><span class="sxs-lookup"><span data-stu-id="d0443-185">string</span></span> | <span data-ttu-id="d0443-186">`az storage` 명령에 사용할 기본 계정 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-186">The default account name to use for `az storage` commands.</span></span> |
| | <span data-ttu-id="d0443-187">key</span><span class="sxs-lookup"><span data-stu-id="d0443-187">key</span></span> | <span data-ttu-id="d0443-188">string</span><span class="sxs-lookup"><span data-stu-id="d0443-188">string</span></span> | <span data-ttu-id="d0443-189">`az storage` 명령에 사용할 기본 계정 키입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-189">The default account key to use for `az storage` commands.</span></span> |
| | <span data-ttu-id="d0443-190">sas\_token</span><span class="sxs-lookup"><span data-stu-id="d0443-190">sas\_token</span></span> | <span data-ttu-id="d0443-191">string</span><span class="sxs-lookup"><span data-stu-id="d0443-191">string</span></span> | <span data-ttu-id="d0443-192">`az storage` 명령에 사용할 기본 SAS 토큰입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-192">The default SAS token to use for `az storage` commands.</span></span> |
| <span data-ttu-id="d0443-193">__batchai__</span><span class="sxs-lookup"><span data-stu-id="d0443-193">__batchai__</span></span> | <span data-ttu-id="d0443-194">storage\_account</span><span class="sxs-lookup"><span data-stu-id="d0443-194">storage\_account</span></span> | <span data-ttu-id="d0443-195">string</span><span class="sxs-lookup"><span data-stu-id="d0443-195">string</span></span> | <span data-ttu-id="d0443-196">`az batchai` 명령에 사용할 기본 스토리지 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-196">The default storage account to use for `az batchai` commands.</span></span> |
| | <span data-ttu-id="d0443-197">storage\_key</span><span class="sxs-lookup"><span data-stu-id="d0443-197">storage\_key</span></span> | <span data-ttu-id="d0443-198">string</span><span class="sxs-lookup"><span data-stu-id="d0443-198">string</span></span> | <span data-ttu-id="d0443-199">`az batchai` 명령에 사용할 기본 스토리지 키입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-199">The default storage key to use for `az batchai` commands.</span></span> |
| <span data-ttu-id="d0443-200">__batch__</span><span class="sxs-lookup"><span data-stu-id="d0443-200">__batch__</span></span> | <span data-ttu-id="d0443-201">계정</span><span class="sxs-lookup"><span data-stu-id="d0443-201">account</span></span> | <span data-ttu-id="d0443-202">string</span><span class="sxs-lookup"><span data-stu-id="d0443-202">string</span></span> | <span data-ttu-id="d0443-203">`az batch` 명령에 사용할 기본 Azure Batch 계정 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-203">The default Azure Batch account name to use for `az batch` commands.</span></span> |
| | <span data-ttu-id="d0443-204">access\_key</span><span class="sxs-lookup"><span data-stu-id="d0443-204">access\_key</span></span> | <span data-ttu-id="d0443-205">string</span><span class="sxs-lookup"><span data-stu-id="d0443-205">string</span></span> | <span data-ttu-id="d0443-206">`az batch` 명령에 사용할 기본 액세스 키입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-206">The default access key to use for `az batch` commands.</span></span> <span data-ttu-id="d0443-207">`aad` 권한 부여와 함께 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-207">Only used with `aad` authorization.</span></span> |
| | <span data-ttu-id="d0443-208">endpoint</span><span class="sxs-lookup"><span data-stu-id="d0443-208">endpoint</span></span> | <span data-ttu-id="d0443-209">string</span><span class="sxs-lookup"><span data-stu-id="d0443-209">string</span></span> | <span data-ttu-id="d0443-210">`az batch` 명령에 대해 연결할 기본 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-210">The default endpoint to connect to for `az batch` commands.</span></span> |
| | <span data-ttu-id="d0443-211">auth\_mode</span><span class="sxs-lookup"><span data-stu-id="d0443-211">auth\_mode</span></span> | <span data-ttu-id="d0443-212">string</span><span class="sxs-lookup"><span data-stu-id="d0443-212">string</span></span> | <span data-ttu-id="d0443-213">`az batch` 명령에 사용할 권한 부여 모드입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-213">The authorization mode to use for `az batch` commands.</span></span> <span data-ttu-id="d0443-214">`shared_key` 또는 `aad`일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-214">Can be `shared_key` or `aad`.</span></span> |

> [!NOTE]
> <span data-ttu-id="d0443-215">구성 파일에 다른 값이 표시될 수 있지만 이는 `az configure`를 포함하여 CLI 명령을 통해 직접 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-215">You may see other values in your configuration file, but these are managed directly through CLI commands, including `az configure`.</span></span> <span data-ttu-id="d0443-216">위의 표에 나열된 것은 사용자가 직접 변경해야 하는 값입니다.</span><span class="sxs-lookup"><span data-stu-id="d0443-216">The ones listed in the table above are the only values you should change yourself.</span></span>

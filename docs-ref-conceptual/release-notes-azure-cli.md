---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/21/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 5b4bcde8c4a66ccc378abc00468cbdb423f07fa4
ms.sourcegitcommit: 3fe3502ec5af89939155285bb5e741b08af604cd
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/24/2019
ms.locfileid: "66197790"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="0dec7-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="0dec7-103">Azure CLI release notes</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="0dec7-104">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="0dec7-104">May 21, 2019</span></span>

<span data-ttu-id="0dec7-105">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="0dec7-105">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-106">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-106">Core</span></span>
* <span data-ttu-id="0dec7-107">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-107">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="0dec7-108">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-108">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="0dec7-109">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-109">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-110">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-110">ACR</span></span>
* <span data-ttu-id="0dec7-111">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-111">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-112">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-112">ACS</span></span>
* <span data-ttu-id="0dec7-113">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-113">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-114">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-114">AppService</span></span>
* <span data-ttu-id="0dec7-115">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-115">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="0dec7-116">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-116">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="0dec7-117">[호환성이 손상되는 변경] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-117">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="0dec7-118">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-118">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="0dec7-119">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-119">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="0dec7-120">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-120">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="0dec7-121">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-121">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-122">BotService</span><span class="sxs-lookup"><span data-stu-id="0dec7-122">BotService</span></span>
* <span data-ttu-id="0dec7-123">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-123">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="0dec7-124">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-124">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-125">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-125">Consumption</span></span>
* <span data-ttu-id="0dec7-126">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-126">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-127">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-127">IoT</span></span>
* <span data-ttu-id="0dec7-128">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-128">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-129">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-129">Network</span></span>
* [호환성이 손상되는 변경]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="0dec7-131">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-131">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="0dec7-132">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-132">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-133">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-133">RDBMS</span></span>
* <span data-ttu-id="0dec7-134">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-134">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="0dec7-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="0dec7-135">RBAC</span></span>
* <span data-ttu-id="0dec7-136">`role assignment`에 관리 그룹 범위가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-136">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-137">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-137">Storage</span></span>
* <span data-ttu-id="0dec7-138">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-138">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="0dec7-139">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="0dec7-139">Compute</span></span>
* <span data-ttu-id="0dec7-140">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-140">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="0dec7-141">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-141">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="0dec7-142">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-142">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="0dec7-143">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-143">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="0dec7-144">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="0dec7-144">May 6, 2019</span></span>

<span data-ttu-id="0dec7-145">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="0dec7-145">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-146">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-146">ACS</span></span>
* <span data-ttu-id="0dec7-147">[호환성이 손상되는 변경] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-147">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="0dec7-148">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-148">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="0dec7-149">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-149">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="0dec7-150">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-150">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-151">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-151">Appservice</span></span>
* <span data-ttu-id="0dec7-152">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-152">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="0dec7-153">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-153">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="0dec7-154">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-154">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="0dec7-155">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-155">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="0dec7-156">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-156">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="0dec7-157">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-157">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="0dec7-158">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-158">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="0dec7-159">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-159">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="0dec7-160">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-160">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="0dec7-161">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-161">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-162">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-162">Batch</span></span>
* <span data-ttu-id="0dec7-163">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-163">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-164">Botservice</span><span class="sxs-lookup"><span data-stu-id="0dec7-164">Botservice</span></span>
* <span data-ttu-id="0dec7-165">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="0dec7-165">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="0dec7-166">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-166">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="0dec7-167">[호환성이 손상되는 변경] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-167">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="0dec7-168">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="0dec7-168">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="0dec7-169">[호환성이 손상되는 변경] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-169">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="0dec7-170">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="0dec7-170">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="0dec7-171">[호환성이 손상되는 변경] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-171">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="0dec7-172">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-172">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="0dec7-173">[호환성이 손상되는 변경] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-173">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="0dec7-174">[호환성이 손상되는 변경] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-174">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="0dec7-175">[호환성이 손상되는 변경] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-175">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="0dec7-176">[호환성이 손상되는 변경] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-176">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="0dec7-177">[호환성이 손상되는 변경] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-177">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="0dec7-178">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-178">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="0dec7-179">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="0dec7-179">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="0dec7-180">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-180">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="0dec7-181">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-181">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="0dec7-182">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-182">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="0dec7-183">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-183">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="0dec7-184">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-184">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="0dec7-185">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-185">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="0dec7-186">구성</span><span class="sxs-lookup"><span data-stu-id="0dec7-186">Configure</span></span>
* <span data-ttu-id="0dec7-187">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-187">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0dec7-188">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0dec7-188">Eventhubs</span></span>
* <span data-ttu-id="0dec7-189">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-189">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="0dec7-190">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-190">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-191">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-191">Network</span></span>
* <span data-ttu-id="0dec7-192">[호환성이 손상되는 변경] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="0dec7-192">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="0dec7-193">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0dec7-193">Policy Insights</span></span>
* <span data-ttu-id="0dec7-194">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-194">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-195">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-195">Role</span></span>
* <span data-ttu-id="0dec7-196">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-196">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="0dec7-197">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0dec7-197">Service Bus</span></span>
* <span data-ttu-id="0dec7-198">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-198">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="0dec7-199">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-199">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="0dec7-200">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-200">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-201">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-201">SQL</span></span>
* <span data-ttu-id="0dec7-202">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-202">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-203">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-203">VM</span></span>
* <span data-ttu-id="0dec7-204">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-204">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="0dec7-205">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-205">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="0dec7-206">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-206">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="0dec7-207">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-207">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="0dec7-208">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-208">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="0dec7-209">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-209">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="0dec7-210">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="0dec7-210">April 23, 2019</span></span>

<span data-ttu-id="0dec7-211">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="0dec7-211">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-212">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-212">ACS</span></span>
* <span data-ttu-id="0dec7-213">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-213">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="0dec7-214">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-214">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-215">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-215">AMS</span></span>
* <span data-ttu-id="0dec7-216">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-216">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-217">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-217">AppService</span></span>
* <span data-ttu-id="0dec7-218">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-218">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="0dec7-219">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-219">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="0dec7-220">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-220">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="0dec7-221">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-221">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="0dec7-222">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-222">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="0dec7-223">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-223">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="0dec7-224">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-224">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="0dec7-225">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-225">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="0dec7-226">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-226">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="0dec7-227">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="0dec7-227">Deployment Manager</span></span>
* <span data-ttu-id="0dec7-228">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="0dec7-228">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="0dec7-229">랩</span><span class="sxs-lookup"><span data-stu-id="0dec7-229">Lab</span></span>
* <span data-ttu-id="0dec7-230">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-230">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-231">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-231">Network</span></span>
* <span data-ttu-id="0dec7-232">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-232">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-233">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-233">Resource</span></span>
* <span data-ttu-id="0dec7-234">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="0dec7-234">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="0dec7-235">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="0dec7-235">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="0dec7-236">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-236">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="0dec7-237">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-237">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-238">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-238">SQL</span></span>
* <span data-ttu-id="0dec7-239">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-239">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="0dec7-240">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-240">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="0dec7-241">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-241">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="0dec7-242">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-242">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-243">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-243">Storage</span></span>
* <span data-ttu-id="0dec7-244">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-244">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-245">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-245">VM</span></span>
* <span data-ttu-id="0dec7-246">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-246">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="0dec7-247">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-247">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="0dec7-248">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-248">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="0dec7-249">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="0dec7-249">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-250">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-250">Core</span></span>
* <span data-ttu-id="0dec7-251">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-251">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-252">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-252">ACR</span></span>
* <span data-ttu-id="0dec7-253">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-253">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-254">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-254">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="0dec7-257">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-257">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="0dec7-258">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-258">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-259">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-259">AppService</span></span>
* <span data-ttu-id="0dec7-260">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-260">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="0dec7-261">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-261">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="0dec7-262">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="0dec7-262">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="0dec7-263">[호환성이 손상되는 변경] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="0dec7-263">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="0dec7-264">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-264">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="0dec7-265">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-265">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="0dec7-266">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-266">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-267">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-267">CDN</span></span>
* <span data-ttu-id="0dec7-268">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-268">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="0dec7-269">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="0dec7-269">Feedback</span></span>
* <span data-ttu-id="0dec7-270">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-270">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="0dec7-271">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-271">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="0dec7-272">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-272">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-273">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-273">Monitor</span></span>
* <span data-ttu-id="0dec7-274">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-274">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="0dec7-275">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-275">Network</span></span>
* <span data-ttu-id="0dec7-276">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-276">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="0dec7-277">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-277">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="0dec7-278">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-278">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="0dec7-279">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-279">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="0dec7-280">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="0dec7-280">PrivateDNS</span></span>
* <span data-ttu-id="0dec7-281">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-281">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-282">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-282">Resource</span></span>
* <span data-ttu-id="0dec7-283">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-283">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-284">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-284">Role</span></span>
* <span data-ttu-id="0dec7-285">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-285">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="0dec7-286">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-286">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-287">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-287">SQL</span></span>
* <span data-ttu-id="0dec7-288">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-288">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-289">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-289">Storage</span></span>
* <span data-ttu-id="0dec7-290">[호환성이 손상되는 변경] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-290">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="0dec7-291">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-291">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="0dec7-292">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-292">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="0dec7-293">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-293">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="0dec7-294">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="0dec7-294">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="0dec7-295">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-295">Core</span></span>
* <span data-ttu-id="0dec7-296">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-296">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="0dec7-297">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-297">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="0dec7-298">클라우드</span><span class="sxs-lookup"><span data-stu-id="0dec7-298">Cloud</span></span>
* <span data-ttu-id="0dec7-299">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-299">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-300">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-300">ACR</span></span>
* <span data-ttu-id="0dec7-301">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-301">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="0dec7-302">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-302">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="0dec7-303">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-303">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="0dec7-304">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-304">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-305">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-305">AppService</span></span>
* <span data-ttu-id="0dec7-306">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-306">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="0dec7-307">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-307">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="0dec7-308">BOT Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-308">BOT Service</span></span>
* <span data-ttu-id="0dec7-309">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-309">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="0dec7-310">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-310">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="0dec7-311">[호환성이 손상되는 변경] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-311">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="0dec7-312">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-312">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-313">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-313">CDN</span></span>
* <span data-ttu-id="0dec7-314">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-314">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="0dec7-316">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-316">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0dec7-317">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-317">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-318">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="0dec7-318">Cosmosdb</span></span>
* <span data-ttu-id="0dec7-319">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-319">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="0dec7-320">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-320">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-321">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-321">Interactive</span></span>
* <span data-ttu-id="0dec7-322">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-322">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-323">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-323">Monitor</span></span>
* <span data-ttu-id="0dec7-324">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-324">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-325">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-325">Network</span></span>
* <span data-ttu-id="0dec7-326">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-326">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-327">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-327">Profile</span></span>
* <span data-ttu-id="0dec7-328">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-328">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="0dec7-329">Postgres</span><span class="sxs-lookup"><span data-stu-id="0dec7-329">Postgres</span></span> 
* <span data-ttu-id="0dec7-330">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-330">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="0dec7-331">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-331">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-332">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-332">Resource</span></span>
* <span data-ttu-id="0dec7-333">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-333">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="0dec7-334">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-334">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="0dec7-335">그래프</span><span class="sxs-lookup"><span data-stu-id="0dec7-335">Graph</span></span>
* <span data-ttu-id="0dec7-336">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-336">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="0dec7-337">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-337">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="0dec7-338">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-338">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="0dec7-339">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-339">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="0dec7-340">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-340">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-341">저장소</span><span class="sxs-lookup"><span data-stu-id="0dec7-341">storage</span></span>
* <span data-ttu-id="0dec7-342">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-342">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="0dec7-343">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-343">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="0dec7-344">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-344">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="0dec7-345">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-345">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-346">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-346">VM</span></span>
* <span data-ttu-id="0dec7-347">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-347">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="0dec7-348">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="0dec7-348">March 12, 2019</span></span>

<span data-ttu-id="0dec7-349">2.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="0dec7-349">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-350">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-350">Core</span></span>

* <span data-ttu-id="0dec7-351">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-351">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-352">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-352">ACR</span></span>

* <span data-ttu-id="0dec7-353">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-353">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-354">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-354">ACS</span></span>

* <span data-ttu-id="0dec7-355">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-355">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="0dec7-356">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-356">AppService</span></span>

* <span data-ttu-id="0dec7-357">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-357">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="0dec7-358">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="0dec7-358">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="0dec7-359">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-359">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="0dec7-360">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-360">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-361">Botservice</span><span class="sxs-lookup"><span data-stu-id="0dec7-361">Botservice</span></span>

* <span data-ttu-id="0dec7-362">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-362">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0dec7-363">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-363">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0dec7-364">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-364">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="0dec7-365">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-365">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-366">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-366">Container</span></span>

* <span data-ttu-id="0dec7-367">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-367">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="0dec7-368">EventHub</span><span class="sxs-lookup"><span data-stu-id="0dec7-368">EventHub</span></span>

* <span data-ttu-id="0dec7-369">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-369">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="0dec7-370">찾기</span><span class="sxs-lookup"><span data-stu-id="0dec7-370">Find</span></span>

* <span data-ttu-id="0dec7-371">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-371">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0dec7-372">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0dec7-372">HDInsight</span></span>

* <span data-ttu-id="0dec7-373">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-373">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-374">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-374">Network</span></span>

* <span data-ttu-id="0dec7-375">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-375">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-376">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0dec7-376">Rdbms</span></span>

* <span data-ttu-id="0dec7-377">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-377">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-378">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-378">Role</span></span>

* <span data-ttu-id="0dec7-379">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-379">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="0dec7-380">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-380">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0dec7-381">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0dec7-381">Service Fabric</span></span>

* <span data-ttu-id="0dec7-382">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-382">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="0dec7-383">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="0dec7-383">February 26, 2019</span></span>

<span data-ttu-id="0dec7-384">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="0dec7-384">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-385">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-385">Core</span></span>

* <span data-ttu-id="0dec7-386">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-386">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-387">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-387">ACR</span></span>

* <span data-ttu-id="0dec7-388">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-388">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="0dec7-389">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-389">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-390">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-390">ACS</span></span>

* <span data-ttu-id="0dec7-391">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-391">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-392">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-392">AppService</span></span>

* <span data-ttu-id="0dec7-393">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-393">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-394">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-394">Batch</span></span>
* <span data-ttu-id="0dec7-395">[호환성이 손상되는 변경] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-395">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="0dec7-396">[호환성이 손상되는 변경] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-396">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="0dec7-397">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-397">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="0dec7-398">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-398">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="0dec7-399">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-399">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="0dec7-400">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-400">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-401">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-401">CosmosDB</span></span>

* <span data-ttu-id="0dec7-402">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-402">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="0dec7-403">Kusto</span><span class="sxs-lookup"><span data-stu-id="0dec7-403">Kusto</span></span>

* <span data-ttu-id="0dec7-404">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-404">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-405">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-405">Network</span></span>

* <span data-ttu-id="0dec7-406">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-406">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="0dec7-407">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-407">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="0dec7-408">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-408">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="0dec7-409">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="0dec7-409">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="0dec7-410">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-410">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="0dec7-411">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-411">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="0dec7-412">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-412">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-413">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-413">Resource</span></span>

* <span data-ttu-id="0dec7-414">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-414">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="0dec7-415">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-415">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="0dec7-416">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-416">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="0dec7-417">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-417">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="0dec7-418">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-418">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-419">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-419">Role</span></span>

* <span data-ttu-id="0dec7-420">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-420">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-421">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-421">VM</span></span>

* <span data-ttu-id="0dec7-422">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-422">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="0dec7-423">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="0dec7-423">February 12, 2019</span></span>

<span data-ttu-id="0dec7-424">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="0dec7-424">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-425">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-425">Core</span></span>

* <span data-ttu-id="0dec7-426">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-426">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="0dec7-427">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-427">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-428">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-428">ACR</span></span>
* <span data-ttu-id="0dec7-429">[호환성이 손상되는 변경] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-429">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="0dec7-430">[호환성이 손상되는 변경] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-430">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-431">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-431">ACS</span></span>
* <span data-ttu-id="0dec7-432">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-432">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="0dec7-433">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-433">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="0dec7-434">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-434">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-435">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-435">AMS</span></span>
* <span data-ttu-id="0dec7-436">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-436">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="0dec7-437">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-437">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-438">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-438">Appservice</span></span>
* <span data-ttu-id="0dec7-439">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-439">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="0dec7-440">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-440">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="0dec7-441">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-441">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="0dec7-442">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-442">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="0dec7-443">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-443">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-444">Botservice</span><span class="sxs-lookup"><span data-stu-id="0dec7-444">Botservice</span></span>
* <span data-ttu-id="0dec7-445">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-445">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="0dec7-446">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-446">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="0dec7-447">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-447">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="0dec7-448">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-448">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="0dec7-449">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-449">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="0dec7-450">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-450">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="0dec7-451">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-451">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="0dec7-452">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-452">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="0dec7-453">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-453">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="0dec7-454">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-454">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="0dec7-455">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0dec7-455">Key Vault</span></span>
* <span data-ttu-id="0dec7-456">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-456">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-457">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-457">Monitor</span></span>
* <span data-ttu-id="0dec7-458">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-458">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-459">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-459">Network</span></span>
* <span data-ttu-id="0dec7-460">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-460">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="0dec7-461">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-461">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="0dec7-462">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-462">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="0dec7-463">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-463">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0dec7-464">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0dec7-464">Policy Insights</span></span>
* <span data-ttu-id="0dec7-465">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-465">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-466">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-466">RDBMS</span></span>
* <span data-ttu-id="0dec7-467">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-467">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="0dec7-468">Redis</span><span class="sxs-lookup"><span data-stu-id="0dec7-468">Redis</span></span>
* <span data-ttu-id="0dec7-469">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-469">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="0dec7-470">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-470">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="0dec7-471">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-471">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="0dec7-472">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-472">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="0dec7-473">[호환성이 손상되는 변경] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-473">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="0dec7-474">[호환성이 손상되는 변경] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-474">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="0dec7-475">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-475">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-476">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-476">Role</span></span>
* <span data-ttu-id="0dec7-477">[호환성이 손상되는 변경] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-477">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="0dec7-478">SQL VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-478">SQL VM</span></span>
* <span data-ttu-id="0dec7-479">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-479">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-480">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-480">VM</span></span>
* <span data-ttu-id="0dec7-481">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-481">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="0dec7-482">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-482">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="0dec7-483">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-483">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="0dec7-484">[호환성이 손상되는 변경] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-484">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="0dec7-485">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="0dec7-485">January 31, 2019</span></span>

<span data-ttu-id="0dec7-486">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="0dec7-486">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-487">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-487">Core</span></span>

* <span data-ttu-id="0dec7-488">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-488">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="0dec7-489">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="0dec7-489">January 28, 2019</span></span>

<span data-ttu-id="0dec7-490">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="0dec7-490">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-491">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-491">ACR</span></span>
* <span data-ttu-id="0dec7-492">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-492">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-493">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-493">ACS</span></span>
* <span data-ttu-id="0dec7-494">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-494">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0dec7-495">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-495">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="0dec7-496">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-496">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-497">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-497">AMS</span></span>
* <span data-ttu-id="0dec7-498">[호환성이 손상되는 변경] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-498">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="0dec7-499">[호환성이 손상되는 변경] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-499">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-500">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-500">Appservice</span></span>
* <span data-ttu-id="0dec7-501">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-501">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="0dec7-502">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 Function Apps에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-502">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="0dec7-503">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-503">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-504">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-504">Container</span></span>
* <span data-ttu-id="0dec7-505">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-505">Added `container start` command</span></span>
* <span data-ttu-id="0dec7-506">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-506">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0dec7-507">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0dec7-507">EventGrid</span></span>
* <span data-ttu-id="0dec7-508">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-508">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="0dec7-509">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-509">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="0dec7-510">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-510">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="0dec7-511">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-511">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="0dec7-512">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-512">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0dec7-513">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0dec7-513">HDInsight</span></span>
* <span data-ttu-id="0dec7-514">[호환성이 손상되는 변경] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-514">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="0dec7-515">[호환성이 손상되는 변경] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-515">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="0dec7-516">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-516">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="0dec7-517">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-517">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="0dec7-518">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-518">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="0dec7-519">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-519">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-520">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-520">IoT</span></span>
* <span data-ttu-id="0dec7-521">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-521">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="0dec7-522">Kusto</span><span class="sxs-lookup"><span data-stu-id="0dec7-522">Kusto</span></span>
* <span data-ttu-id="0dec7-523">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-523">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-524">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-524">Monitor</span></span>
* <span data-ttu-id="0dec7-525">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-525">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-526">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-526">Profile</span></span>
* <span data-ttu-id="0dec7-527">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-527">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-528">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-528">Network</span></span>
* <span data-ttu-id="0dec7-529">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-529">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="0dec7-530">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-530">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-531">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-531">Resource</span></span>
* <span data-ttu-id="0dec7-532">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-532">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="0dec7-533">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-533">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="0dec7-534">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="0dec7-534">SQL Virtual Machine</span></span>
* <span data-ttu-id="0dec7-535">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-535">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-536">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-536">Storage</span></span>
* <span data-ttu-id="0dec7-537">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-537">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="0dec7-538">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-538">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-539">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-539">VM</span></span>
* <span data-ttu-id="0dec7-540">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-540">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="0dec7-541">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-541">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="0dec7-542">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="0dec7-542">January 15, 2019</span></span>

<span data-ttu-id="0dec7-543">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="0dec7-543">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-544">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-544">ACR</span></span>
* <span data-ttu-id="0dec7-545">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-545">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="0dec7-546">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-546">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="0dec7-547">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="0dec7-547">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="0dec7-548">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-548">ACS</span></span>
* <span data-ttu-id="0dec7-549">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-549">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-550">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-550">Appservice</span></span>
* <span data-ttu-id="0dec7-551">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-551">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="0dec7-552">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-552">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="0dec7-553">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-553">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="0dec7-554">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-554">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-555">Botservice</span><span class="sxs-lookup"><span data-stu-id="0dec7-555">Botservice</span></span>
* <span data-ttu-id="0dec7-556">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-556">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="0dec7-557">구성</span><span class="sxs-lookup"><span data-stu-id="0dec7-557">Configure</span></span>
* <span data-ttu-id="0dec7-558">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-558">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-559">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-559">CosmosDB</span></span>
* <span data-ttu-id="0dec7-560">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-560">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0dec7-561">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0dec7-561">HDInsight</span></span>
* <span data-ttu-id="0dec7-562">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-562">Added commands for managing applications</span></span>
* <span data-ttu-id="0dec7-563">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-563">Added commands for managing script actions</span></span>
* <span data-ttu-id="0dec7-564">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-564">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="0dec7-565">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-565">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="0dec7-566">[호환성이 손상되는 변경] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-566">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-567">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-567">Network</span></span>
* <span data-ttu-id="0dec7-568">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-568">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="0dec7-569">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-569">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="0dec7-570">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-570">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="0dec7-571">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-571">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-572">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-572">Role</span></span>
* <span data-ttu-id="0dec7-573">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-573">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="0dec7-574">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-574">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="0dec7-575">보안</span><span class="sxs-lookup"><span data-stu-id="0dec7-575">Security</span></span>
* <span data-ttu-id="0dec7-576">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-576">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-577">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-577">Storage</span></span>
* <span data-ttu-id="0dec7-578">[호환성이 손상되는 변경] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-578">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="0dec7-579">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-579">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="0dec7-580">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-580">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="0dec7-581">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-581">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="0dec7-582">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-582">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-583">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-583">VM</span></span>
* <span data-ttu-id="0dec7-584">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-584">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="0dec7-585">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-585">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0dec7-586">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-586">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="0dec7-587">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-587">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="0dec7-588">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-588">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="0dec7-589">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-589">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="0dec7-590">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="0dec7-590">December 20, 2018</span></span>

<span data-ttu-id="0dec7-591">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="0dec7-591">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="0dec7-592">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-592">Appservice</span></span>
* <span data-ttu-id="0dec7-593">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-593">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="0dec7-594">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-594">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="0dec7-595">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-595">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0dec7-596">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="0dec7-596">IoTCentral</span></span>
* <span data-ttu-id="0dec7-597">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-597">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-598">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-598">Role</span></span>
* <span data-ttu-id="0dec7-599">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-599">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-600">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-600">SQL</span></span>
* <span data-ttu-id="0dec7-601">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-601">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-602">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-602">VM</span></span>
* <span data-ttu-id="0dec7-603">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-603">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="0dec7-604">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="0dec7-604">December 18, 2018</span></span>

<span data-ttu-id="0dec7-605">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="0dec7-605">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="0dec7-606">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-606">ACR</span></span>
* <span data-ttu-id="0dec7-607">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-607">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="0dec7-608">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="0dec7-608">Condensed the table layout for task list</span></span>
* <span data-ttu-id="0dec7-609">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-609">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-610">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-610">ACS</span></span>
* <span data-ttu-id="0dec7-611">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-611">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0dec7-612">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="0dec7-612">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="0dec7-613">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-613">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="0dec7-614">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-614">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="0dec7-615">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-615">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="0dec7-616">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="0dec7-616">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-617">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-617">Appservice</span></span>
* <span data-ttu-id="0dec7-618">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-618">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="0dec7-619">Botservice</span><span class="sxs-lookup"><span data-stu-id="0dec7-619">Botservice</span></span>
* <span data-ttu-id="0dec7-620">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-620">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="0dec7-621">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="0dec7-621">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="0dec7-622">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="0dec7-622">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="0dec7-623">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="0dec7-623">Reduced Kudu network calls</span></span>
* <span data-ttu-id="0dec7-624">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-624">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-625">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-625">Consumption</span></span>
* <span data-ttu-id="0dec7-626">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-626">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-627">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-627">CosmosDB</span></span>
* <span data-ttu-id="0dec7-628">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-628">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="0dec7-629">지도</span><span class="sxs-lookup"><span data-stu-id="0dec7-629">Maps</span></span>
* <span data-ttu-id="0dec7-630">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-630">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-631">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-631">Network</span></span>
* <span data-ttu-id="0dec7-632">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-632">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="0dec7-633">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="0dec7-633">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-634">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-634">Resource</span></span>
* <span data-ttu-id="0dec7-635">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-635">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="0dec7-636">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-636">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-637">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-637">Storage</span></span>
*  <span data-ttu-id="0dec7-638">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-638">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-639">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-639">VM</span></span>
* <span data-ttu-id="0dec7-640">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-640">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="0dec7-641">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="0dec7-641">December 4, 2018</span></span>

<span data-ttu-id="0dec7-642">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="0dec7-642">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="0dec7-643">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-643">Core</span></span>
* <span data-ttu-id="0dec7-644">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-644">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="0dec7-645">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-645">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-646">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-646">Appservice</span></span>
* <span data-ttu-id="0dec7-647">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-647">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="0dec7-648">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-648">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-649">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-649">Network</span></span>
* <span data-ttu-id="0dec7-650">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-650">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-651">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-651">Role</span></span>
* <span data-ttu-id="0dec7-652">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-652">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="0dec7-653">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-653">VM</span></span>
* <span data-ttu-id="0dec7-654">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-654">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="0dec7-655">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-655">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="0dec7-656">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-656">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="0dec7-657">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-657">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="0dec7-658">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="0dec7-658">November 20, 2018</span></span>

<span data-ttu-id="0dec7-659">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="0dec7-659">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="0dec7-660">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-660">Core</span></span>
* <span data-ttu-id="0dec7-661">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-661">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-662">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-662">ACR</span></span>
* <span data-ttu-id="0dec7-663">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-663">Added context token to task step</span></span>
* <span data-ttu-id="0dec7-664">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-664">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="0dec7-665">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-665">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-666">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-666">Appservice</span></span>
* <span data-ttu-id="0dec7-667">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-667">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="0dec7-668">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-668">Updated the default `node_version`.</span></span> <span data-ttu-id="0dec7-669">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-669">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="0dec7-670">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-670">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="0dec7-671">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-671">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0dec7-672">IotCentral</span><span class="sxs-lookup"><span data-stu-id="0dec7-672">IotCentral</span></span>
* <span data-ttu-id="0dec7-673">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-673">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-674">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0dec7-674">KeyVault</span></span>
* <span data-ttu-id="0dec7-675">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-675">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-676">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-676">Network</span></span>
* <span data-ttu-id="0dec7-677">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-677">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="0dec7-678">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="0dec7-678">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="0dec7-679">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-679">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="0dec7-680">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="0dec7-680">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-681">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0dec7-681">Rdbms</span></span>
* <span data-ttu-id="0dec7-682">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-682">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="0dec7-683">Rbac</span><span class="sxs-lookup"><span data-stu-id="0dec7-683">Rbac</span></span>
* <span data-ttu-id="0dec7-684">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-684">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="0dec7-685">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-685">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="0dec7-686">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-686">Storage</span></span>
* <span data-ttu-id="0dec7-687">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-687">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="0dec7-688">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-688">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="0dec7-689">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-689">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="0dec7-690">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-690">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-691">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-691">VM</span></span>
* <span data-ttu-id="0dec7-692">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-692">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="0dec7-693">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-693">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="0dec7-694">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-694">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="0dec7-695">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-695">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="0dec7-696">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-696">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="0dec7-697">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-697">Added `snapshot wait` command</span></span>
* <span data-ttu-id="0dec7-698">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-698">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="0dec7-699">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="0dec7-699">November 6, 2018</span></span>

<span data-ttu-id="0dec7-700">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="0dec7-700">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-701">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-701">Core</span></span>
* <span data-ttu-id="0dec7-702">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-702">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-703">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-703">ACR</span></span>
* <span data-ttu-id="0dec7-704">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-704">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="0dec7-705">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-705">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-706">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-706">ACS</span></span>
* <span data-ttu-id="0dec7-707">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-707">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="0dec7-708">Advisor</span><span class="sxs-lookup"><span data-stu-id="0dec7-708">Advisor</span></span>
* <span data-ttu-id="0dec7-709">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-709">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-710">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-710">AMS</span></span>
* <span data-ttu-id="0dec7-711">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="0dec7-711">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="0dec7-712">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="0dec7-712">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="0dec7-713">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-713">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="0dec7-714">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-714">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="0dec7-715">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-715">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="0dec7-716">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-716">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="0dec7-717">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-717">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="0dec7-718">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-718">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="0dec7-719">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-719">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="0dec7-720">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-720">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="0dec7-721">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-721">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="0dec7-722">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-722">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="0dec7-723">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="0dec7-723">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="0dec7-724">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="0dec7-724">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="0dec7-725">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-725">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="0dec7-726">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-726">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="0dec7-727">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-727">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-728">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-728">AppService</span></span>
* <span data-ttu-id="0dec7-729">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-729">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="0dec7-730">구성</span><span class="sxs-lookup"><span data-stu-id="0dec7-730">Configure</span></span>
* <span data-ttu-id="0dec7-731">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-731">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-732">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-732">Container</span></span>
* <span data-ttu-id="0dec7-733">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-733">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="0dec7-734">EventHub</span><span class="sxs-lookup"><span data-stu-id="0dec7-734">EventHub</span></span>
* <span data-ttu-id="0dec7-735">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-735">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-736">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-736">Interactive</span></span>
* <span data-ttu-id="0dec7-737">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-737">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-738">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-738">Monitor</span></span>
* <span data-ttu-id="0dec7-739">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-739">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-740">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-740">Network</span></span>
* <span data-ttu-id="0dec7-741">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-741">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="0dec7-742">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-742">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="0dec7-743">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-743">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="0dec7-744">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-744">Profile</span></span>
* <span data-ttu-id="0dec7-745">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-745">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-746">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-746">RDBMS</span></span>
* <span data-ttu-id="0dec7-747">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-747">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-748">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-748">Resource</span></span>
* <span data-ttu-id="0dec7-749">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-749">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-750">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-750">Role</span></span>
* <span data-ttu-id="0dec7-751">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-751">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="0dec7-752">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-752">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="0dec7-753">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-753">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-754">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-754">Storage</span></span>
* <span data-ttu-id="0dec7-755">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-755">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-756">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-756">VM</span></span>
* <span data-ttu-id="0dec7-757">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-757">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="0dec7-758">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-758">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="0dec7-759">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-759">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="0dec7-760">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-760">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="0dec7-761">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="0dec7-761">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="0dec7-762">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-762">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="0dec7-763">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="0dec7-763">October 23, 2018</span></span>

<span data-ttu-id="0dec7-764">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="0dec7-764">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-765">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-765">Core</span></span>
* <span data-ttu-id="0dec7-766">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-766">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="0dec7-767">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-767">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-768">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-768">ACR</span></span>
* <span data-ttu-id="0dec7-769">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-769">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-770">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-770">CDN</span></span>
* <span data-ttu-id="0dec7-771">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-771">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0dec7-772">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-772">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-773">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-773">Container</span></span>
* <span data-ttu-id="0dec7-774">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-774">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="0dec7-775">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-775">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="0dec7-776">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-776">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="0dec7-777">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-777">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="0dec7-778">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-778">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="0dec7-779">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-779">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="0dec7-780">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-780">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-781">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-781">CosmosDB</span></span>
* <span data-ttu-id="0dec7-782">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-782">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-783">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-783">Interactive</span></span>
* <span data-ttu-id="0dec7-784">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-784">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="0dec7-785">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0dec7-785">IoT Central</span></span>
* <span data-ttu-id="0dec7-786">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-786">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="0dec7-787">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-787">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-788">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-788">Monitor</span></span>
* <span data-ttu-id="0dec7-789">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0dec7-789">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="0dec7-790">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-790">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="0dec7-791">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-791">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0dec7-792">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-792">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="0dec7-793">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-793">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="0dec7-794">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-794">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="0dec7-795">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0dec7-795">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="0dec7-796">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-796">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0dec7-797">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-797">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="0dec7-798">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-798">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-799">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-799">Network</span></span>
* <span data-ttu-id="0dec7-800">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-800">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="0dec7-801">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-801">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="0dec7-802">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0dec7-802">ServiceBus</span></span>
* <span data-ttu-id="0dec7-803">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-803">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-804">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-804">SQL</span></span>
* <span data-ttu-id="0dec7-805">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-805">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-806">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-806">Storage</span></span>
* <span data-ttu-id="0dec7-807">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-807">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="0dec7-808">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-808">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-809">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-809">VM</span></span>
* <span data-ttu-id="0dec7-810">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-810">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="0dec7-811">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-811">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="0dec7-812">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-812">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="0dec7-813">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="0dec7-813">October 16, 2018</span></span>

<span data-ttu-id="0dec7-814">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="0dec7-814">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-815">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-815">VM</span></span>
* <span data-ttu-id="0dec7-816">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-816">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="0dec7-817">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="0dec7-817">October 9, 2018</span></span>

<span data-ttu-id="0dec7-818">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="0dec7-818">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-819">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-819">Core</span></span>
* <span data-ttu-id="0dec7-820">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-820">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-821">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-821">ACR</span></span>
* <span data-ttu-id="0dec7-822">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-822">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-823">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-823">ACS</span></span>
* <span data-ttu-id="0dec7-824">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="0dec7-824">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="0dec7-825">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-825">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="0dec7-826">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-826">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="0dec7-827">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-827">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-828">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-828">Container</span></span>
* <span data-ttu-id="0dec7-829">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-829">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="0dec7-830">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-830">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="0dec7-831">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="0dec7-831">Event Hub</span></span>
* <span data-ttu-id="0dec7-832">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-832">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="0dec7-833">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-833">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="0dec7-834">확장</span><span class="sxs-lookup"><span data-stu-id="0dec7-834">Extensions</span></span>
* <span data-ttu-id="0dec7-835">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-835">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0dec7-836">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0dec7-836">HDInsight</span></span>
* <span data-ttu-id="0dec7-837">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-837">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-838">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-838">IoT</span></span>
* <span data-ttu-id="0dec7-839">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-839">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-840">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0dec7-840">KeyVault</span></span>
* <span data-ttu-id="0dec7-841">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-841">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-842">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-842">Network</span></span>
* <span data-ttu-id="0dec7-843">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-843">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="0dec7-844">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="0dec7-844">See #6052</span></span>
* <span data-ttu-id="0dec7-845">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0dec7-845">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="0dec7-846">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-846">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="0dec7-847">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-847">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="0dec7-848">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-848">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="0dec7-849">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-849">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="0dec7-850">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-850">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-851">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-851">Role</span></span>
* <span data-ttu-id="0dec7-852">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-852">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="0dec7-853">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-853">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="0dec7-854">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-854">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="0dec7-855">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-855">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="0dec7-856">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0dec7-856">Service Bus</span></span>
* <span data-ttu-id="0dec7-857">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-857">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-858">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-858">VM</span></span>
* <span data-ttu-id="0dec7-859">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-859">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="0dec7-860">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-860">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="0dec7-861">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-861">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="0dec7-862">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-862">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="0dec7-863">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-863">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="0dec7-864">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-864">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="0dec7-865">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="0dec7-865">September 21, 2018</span></span>

<span data-ttu-id="0dec7-866">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="0dec7-866">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-867">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-867">ACR</span></span>
* <span data-ttu-id="0dec7-868">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-868">Added ACR Task commands</span></span>
* <span data-ttu-id="0dec7-869">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-869">Added quick run command</span></span>
* <span data-ttu-id="0dec7-870">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-870">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="0dec7-871">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-871">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="0dec7-872">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-872">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="0dec7-873">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-873">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-874">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-874">ACS</span></span>
* <span data-ttu-id="0dec7-875">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-875">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="0dec7-876">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-876">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-877">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-877">AppService</span></span>

* <span data-ttu-id="0dec7-878">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-878">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="0dec7-879">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-879">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="0dec7-880">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-880">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="0dec7-881">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-881">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-882">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-882">Batch</span></span>
* <span data-ttu-id="0dec7-883">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-883">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="0dec7-884">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-884">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="0dec7-885">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-885">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="0dec7-886">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-886">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0dec7-887">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0dec7-887">Batch AI</span></span> 
* <span data-ttu-id="0dec7-888">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-888">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0dec7-889">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0dec7-889">Cognitive Services</span></span>
* <span data-ttu-id="0dec7-890">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-890">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="0dec7-891">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-891">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="0dec7-892">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-892">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="0dec7-893">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-893">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="0dec7-894">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-894">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="0dec7-895">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-895">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-896">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-896">Container</span></span>
* <span data-ttu-id="0dec7-897">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-897">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="0dec7-898">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-898">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="0dec7-899">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-899">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="0dec7-900">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-900">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="0dec7-901">Datalake</span><span class="sxs-lookup"><span data-stu-id="0dec7-901">Datalake</span></span>
* <span data-ttu-id="0dec7-902">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-902">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="0dec7-903">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="0dec7-903">Interactive Shell</span></span>
* <span data-ttu-id="0dec7-904">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-904">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="0dec7-905">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-905">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-906">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-906">IoT</span></span>
* <span data-ttu-id="0dec7-907">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-907">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="0dec7-908">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0dec7-908">Key Vault</span></span>
* <span data-ttu-id="0dec7-909">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-909">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-910">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-910">Network</span></span>
* <span data-ttu-id="0dec7-911">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-911">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="0dec7-912">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-912">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="0dec7-913">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-913">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="0dec7-914">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-914">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="0dec7-915">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-915">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="0dec7-916">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-916">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="0dec7-917">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-917">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="0dec7-918">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-918">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="0dec7-919">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-919">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="0dec7-920">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-920">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="0dec7-921">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-921">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="0dec7-922">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-922">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="0dec7-923">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-923">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="0dec7-924">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-924">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="0dec7-925">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-925">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="0dec7-926">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-926">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="0dec7-927">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-927">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="0dec7-928">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-928">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-929">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-929">RDBMS</span></span>
* <span data-ttu-id="0dec7-930">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-930">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="0dec7-931">예약</span><span class="sxs-lookup"><span data-stu-id="0dec7-931">Reservation</span></span>
* <span data-ttu-id="0dec7-932">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-932">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="0dec7-933">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-933">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="0dec7-934">앱 관리</span><span class="sxs-lookup"><span data-stu-id="0dec7-934">Manage App</span></span>
* <span data-ttu-id="0dec7-935">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-935">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="0dec7-936">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-936">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-937">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-937">Role</span></span>
* <span data-ttu-id="0dec7-938">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-938">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="0dec7-939">SignalR</span><span class="sxs-lookup"><span data-stu-id="0dec7-939">SignalR</span></span>
* <span data-ttu-id="0dec7-940">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-940">First release</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-941">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-941">Storage</span></span>
* <span data-ttu-id="0dec7-942">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-942">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="0dec7-943">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-943">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-944">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-944">VM</span></span>
* <span data-ttu-id="0dec7-945">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="0dec7-945">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="0dec7-946">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-946">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="0dec7-947">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="0dec7-947">August 28, 2018</span></span>

<span data-ttu-id="0dec7-948">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="0dec7-948">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-949">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-949">Core</span></span>

* <span data-ttu-id="0dec7-950">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-950">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="0dec7-951">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-951">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-952">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-952">ACR</span></span>

* <span data-ttu-id="0dec7-953">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-953">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="0dec7-954">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-954">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-955">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-955">ACS</span></span>

* <span data-ttu-id="0dec7-956">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-956">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="0dec7-957">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-957">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-958">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-958">AppService</span></span>

* <span data-ttu-id="0dec7-959">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-959">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="0dec7-960">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-960">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="0dec7-961">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-961">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="0dec7-962">Backup</span><span class="sxs-lookup"><span data-stu-id="0dec7-962">Backup</span></span>

* <span data-ttu-id="0dec7-963">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-963">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="0dec7-964">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="0dec7-964">Bot Service</span></span>

* <span data-ttu-id="0dec7-965">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-965">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0dec7-966">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0dec7-966">Cognitive Services</span></span>

* <span data-ttu-id="0dec7-967">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-967">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-968">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-968">IoT</span></span>

* <span data-ttu-id="0dec7-969">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-969">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-970">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-970">Monitor</span></span>

* <span data-ttu-id="0dec7-971">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-971">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="0dec7-972">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="0dec7-972">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-973">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-973">Network</span></span>

* <span data-ttu-id="0dec7-974">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-974">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-975">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-975">Resource</span></span>

* <span data-ttu-id="0dec7-976">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-976">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-977">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-977">Storage</span></span>

* <span data-ttu-id="0dec7-978">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-978">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-979">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-979">VM</span></span>

* <span data-ttu-id="0dec7-980">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-980">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="0dec7-981">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0dec7-981">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="0dec7-982">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="0dec7-982">Auguest 14, 2018</span></span>

<span data-ttu-id="0dec7-983">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="0dec7-983">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-984">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-984">Core</span></span>

* <span data-ttu-id="0dec7-985">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-985">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="0dec7-986">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="0dec7-986">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="0dec7-987">원격 분석</span><span class="sxs-lookup"><span data-stu-id="0dec7-987">Telemetry</span></span>

* <span data-ttu-id="0dec7-988">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="0dec7-988">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-989">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-989">ACR</span></span>

* <span data-ttu-id="0dec7-990">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-990">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="0dec7-991">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-991">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-992">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-992">ACS</span></span>

* <span data-ttu-id="0dec7-993">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-993">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="0dec7-994">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-994">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="0dec7-995">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-995">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="0dec7-996">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-996">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="0dec7-997">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-997">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="0dec7-998">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-998">AppService</span></span>

* <span data-ttu-id="0dec7-999">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-999">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="0dec7-1000">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1000">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="0dec7-1001">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1001">BatchAI</span></span>

* <span data-ttu-id="0dec7-1002">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1002">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="0dec7-1003">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1003">Container</span></span>

* <span data-ttu-id="0dec7-1004">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1004">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="0dec7-1005">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-1005">IoT</span></span>

* <span data-ttu-id="0dec7-1006">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="0dec7-1006">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="0dec7-1007">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1007">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="0dec7-1008">Iot Central</span><span class="sxs-lookup"><span data-stu-id="0dec7-1008">Iot Central</span></span>

* <span data-ttu-id="0dec7-1009">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1009">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-1010">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0dec7-1010">KeyVault</span></span>


* <span data-ttu-id="0dec7-1011">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1011">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="0dec7-1012">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1012">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="0dec7-1013">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1013">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="0dec7-1014">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1014">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="0dec7-1015">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1015">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="0dec7-1016">릴레이</span><span class="sxs-lookup"><span data-stu-id="0dec7-1016">Relay</span></span>

* <span data-ttu-id="0dec7-1017">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1017">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1018">Sql</span><span class="sxs-lookup"><span data-stu-id="0dec7-1018">Sql</span></span>

* <span data-ttu-id="0dec7-1019">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1019">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1020">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1020">Storage</span></span>

* <span data-ttu-id="0dec7-1021">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1021">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="0dec7-1022">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1022">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="0dec7-1023">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1023">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="0dec7-1024">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1024">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="0dec7-1025">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1025">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1026">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1026">VM</span></span>

* <span data-ttu-id="0dec7-1027">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1027">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="0dec7-1028">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1028">July 31, 2018</span></span>

<span data-ttu-id="0dec7-1029">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="0dec7-1029">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1030">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1030">ACR</span></span>

* <span data-ttu-id="0dec7-1031">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1031">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="0dec7-1032">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1032">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1033">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1033">ACS</span></span>

* <span data-ttu-id="0dec7-1034">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1034">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1035">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1035">Batch</span></span>

* <span data-ttu-id="0dec7-1036">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1036">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1037">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1037">Container</span></span>

* <span data-ttu-id="0dec7-1038">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1038">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1039">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1039">Network</span></span>

* <span data-ttu-id="0dec7-1040">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1040">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="0dec7-1041">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1041">Resource</span></span>

* <span data-ttu-id="0dec7-1042">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1042">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="0dec7-1043">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1043">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1044">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1044">Role</span></span>

* <span data-ttu-id="0dec7-1045">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1045">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="0dec7-1046">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1046">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="0dec7-1047">검색</span><span class="sxs-lookup"><span data-stu-id="0dec7-1047">Search</span></span>

* <span data-ttu-id="0dec7-1048">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1048">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="0dec7-1049">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0dec7-1049">Service Bus</span></span>

* <span data-ttu-id="0dec7-1050">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1050">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="0dec7-1051">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1051">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="0dec7-1052">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1052">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="0dec7-1053">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1053">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1054">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1054">Storage</span></span>

* <span data-ttu-id="0dec7-1055">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1055">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="0dec7-1056">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="0dec7-1056">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1057">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1057">VM</span></span>

* <span data-ttu-id="0dec7-1058">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1058">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="0dec7-1059">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1059">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="0dec7-1060">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1060">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="0dec7-1061">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1061">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="0dec7-1062">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1062">July 18, 2018</span></span>

<span data-ttu-id="0dec7-1063">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="0dec7-1063">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1064">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1064">Core</span></span>

* <span data-ttu-id="0dec7-1065">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1065">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="0dec7-1066">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1066">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="0dec7-1067">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1067">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1068">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1068">ACR</span></span>

* <span data-ttu-id="0dec7-1069">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1069">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="0dec7-1070">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1070">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="0dec7-1071">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1071">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="0dec7-1072">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1072">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1073">ACS</span></span>

* <span data-ttu-id="0dec7-1074">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1074">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1075">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-1075">AppService</span></span>

* <span data-ttu-id="0dec7-1076">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1076">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1077">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1077">Batch</span></span>

* <span data-ttu-id="0dec7-1078">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1078">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="0dec7-1079">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1079">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0dec7-1080">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1080">Batch AI</span></span>

* <span data-ttu-id="0dec7-1081">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1081">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1082">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1082">Container</span></span>

* <span data-ttu-id="0dec7-1083">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1083">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="0dec7-1084">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1084">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1085">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1085">Network</span></span>

* <span data-ttu-id="0dec7-1086">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1086">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="0dec7-1087">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1087">Added `network nic wait`</span></span>
* <span data-ttu-id="0dec7-1088">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1088">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="0dec7-1089">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1089">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="0dec7-1090">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1090">Resource</span></span>

* <span data-ttu-id="0dec7-1091">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1091">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="0dec7-1092">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1092">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="0dec7-1093">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1093">Added `deployment wait` command</span></span>
* <span data-ttu-id="0dec7-1094">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1094">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1095">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1095">SQL</span></span>

* <span data-ttu-id="0dec7-1096">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1096">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="0dec7-1097">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1097">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="0dec7-1098">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1098">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1099">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1099">Storage</span></span>

* <span data-ttu-id="0dec7-1100">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1100">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1101">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1101">VM</span></span>

* <span data-ttu-id="0dec7-1102">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1102">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="0dec7-1103">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1103">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="0dec7-1104">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1104">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0dec7-1105">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1105">July 3, 2018</span></span>

<span data-ttu-id="0dec7-1106">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="0dec7-1106">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="0dec7-1107">AKS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1107">AKS</span></span>

* <span data-ttu-id="0dec7-1108">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1108">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0dec7-1109">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1109">July 3, 2018</span></span>

<span data-ttu-id="0dec7-1110">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="0dec7-1110">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1111">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1111">Core</span></span>

* <span data-ttu-id="0dec7-1112">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1112">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1113">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1113">ACR</span></span>

* <span data-ttu-id="0dec7-1114">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1114">Added polling build status</span></span>
* <span data-ttu-id="0dec7-1115">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1115">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="0dec7-1116">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1116">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1117">ACS</span></span>

* <span data-ttu-id="0dec7-1118">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1118">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="0dec7-1119">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1119">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="0dec7-1120">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1120">Updated options for `aks browse` command.</span></span> <span data-ttu-id="0dec7-1121">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1121">Added `--listen-port` support</span></span>
* <span data-ttu-id="0dec7-1122">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1122">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="0dec7-1123">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1123">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="0dec7-1124">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1124">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-1125">AppService</span></span>

* <span data-ttu-id="0dec7-1126">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1126">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="0dec7-1127">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1127">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="0dec7-1128">Backup</span><span class="sxs-lookup"><span data-stu-id="0dec7-1128">Backup</span></span>

* <span data-ttu-id="0dec7-1129">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1129">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="0dec7-1130">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1130">BatchAI</span></span>

* <span data-ttu-id="0dec7-1131">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1131">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="0dec7-1132">클라우드</span><span class="sxs-lookup"><span data-stu-id="0dec7-1132">Cloud</span></span>

* <span data-ttu-id="0dec7-1133">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1133">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1134">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1134">Container</span></span>

* <span data-ttu-id="0dec7-1135">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1135">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="0dec7-1136">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1136">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="0dec7-1137">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1137">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1138">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1138">Extension</span></span>

* <span data-ttu-id="0dec7-1139">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1139">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1140">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1140">Network</span></span>

* <span data-ttu-id="0dec7-1141">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="0dec7-1141">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-1142">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0dec7-1142">Rdbms</span></span>

* <span data-ttu-id="0dec7-1143">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1143">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1144">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1144">Resource</span></span>

* <span data-ttu-id="0dec7-1145">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1145">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1146">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1146">VM</span></span>

* <span data-ttu-id="0dec7-1147">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1147">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="0dec7-1148">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1148">June 25, 2018</span></span>

<span data-ttu-id="0dec7-1149">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="0dec7-1149">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="0dec7-1150">CLI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1150">CLI</span></span>

* <span data-ttu-id="0dec7-1151">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1151">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="0dec7-1152">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1152">June 19, 2018</span></span>

<span data-ttu-id="0dec7-1153">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="0dec7-1153">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1154">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1154">Core</span></span>

* <span data-ttu-id="0dec7-1155">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1155">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1156">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1156">ACR</span></span>

* <span data-ttu-id="0dec7-1157">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1157">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="0dec7-1158">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1158">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1159">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1159">ACS</span></span>

* <span data-ttu-id="0dec7-1160">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1160">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="0dec7-1161">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1161">Added `--update` support</span></span>
* <span data-ttu-id="0dec7-1162">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1162">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="0dec7-1163">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="0dec7-1163">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="0dec7-1164">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1164">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="0dec7-1165">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1165">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="0dec7-1166">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1166">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="0dec7-1167">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1167">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1168">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-1168">AppService</span></span>

* <span data-ttu-id="0dec7-1169">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1169">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="0dec7-1170">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1170">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1171">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1171">Batch</span></span>

* <span data-ttu-id="0dec7-1172">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1172">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0dec7-1173">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1173">Batch AI</span></span>

* <span data-ttu-id="0dec7-1174">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1174">Added support for workspaces.</span></span> <span data-ttu-id="0dec7-1175">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1175">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="0dec7-1176">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1176">Added support for experiments.</span></span> <span data-ttu-id="0dec7-1177">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1177">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="0dec7-1178">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1178">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="0dec7-1179">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1179">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="0dec7-1180">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1180">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="0dec7-1181">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1181">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="0dec7-1182">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="0dec7-1182">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="0dec7-1183">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="0dec7-1183">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="0dec7-1184">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1184">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="0dec7-1185">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="0dec7-1185">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="0dec7-1186">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1186">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="0dec7-1187">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="0dec7-1187">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="0dec7-1188">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1188">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="0dec7-1189">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1189">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="0dec7-1190">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1190">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="0dec7-1191">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="0dec7-1191">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="0dec7-1192">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0dec7-1192">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="0dec7-1193">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0dec7-1193">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0dec7-1194">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0dec7-1194">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0dec7-1195">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0dec7-1195">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="0dec7-1196">지도</span><span class="sxs-lookup"><span data-stu-id="0dec7-1196">Maps</span></span>

* <span data-ttu-id="0dec7-1197">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1197">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1198">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1198">Network</span></span>

* <span data-ttu-id="0dec7-1199">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1199">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="0dec7-1200">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1200">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="0dec7-1201">#6502</span><span class="sxs-lookup"><span data-stu-id="0dec7-1201">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="0dec7-1202">예약</span><span class="sxs-lookup"><span data-stu-id="0dec7-1202">Reservations</span></span>

* <span data-ttu-id="0dec7-1203">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1203">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="0dec7-1204">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1204">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="0dec7-1205">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1205">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="0dec7-1206">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1206">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="0dec7-1207">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1207">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="0dec7-1208">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1208">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1209">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1209">Role</span></span>

* <span data-ttu-id="0dec7-1210">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="0dec7-1210">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1211">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1211">SQL</span></span>

* <span data-ttu-id="0dec7-1212">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1212">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1213">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1213">Storage</span></span>

* <span data-ttu-id="0dec7-1214">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1214">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1215">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1215">VM</span></span>

* <span data-ttu-id="0dec7-1216">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-1216">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="0dec7-1217">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1217">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="0dec7-1218">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1218">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0dec7-1219">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1219">June 13, 2018</span></span>

<span data-ttu-id="0dec7-1220">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="0dec7-1220">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1221">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1221">Core</span></span>

* <span data-ttu-id="0dec7-1222">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="0dec7-1222">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0dec7-1223">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1223">June 13, 2018</span></span>

<span data-ttu-id="0dec7-1224">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="0dec7-1224">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="0dec7-1225">AKS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1225">AKS</span></span>

* <span data-ttu-id="0dec7-1226">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1226">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="0dec7-1227">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="0dec7-1227">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="0dec7-1228">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1228">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="0dec7-1229">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1229">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="0dec7-1230">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1230">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1231">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-1231">AppService</span></span>

* <span data-ttu-id="0dec7-1232">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1232">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0dec7-1233">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1233">June 5, 2018</span></span>

<span data-ttu-id="0dec7-1234">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="0dec7-1234">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1235">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1235">Interactive</span></span>

* <span data-ttu-id="0dec7-1236">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1236">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0dec7-1237">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1237">June 5, 2018</span></span>

<span data-ttu-id="0dec7-1238">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="0dec7-1238">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1239">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1239">Core</span></span>

* <span data-ttu-id="0dec7-1240">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1240">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="0dec7-1241">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1241">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1242">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1242">ACR</span></span>

* <span data-ttu-id="0dec7-1243">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1243">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="0dec7-1244">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1244">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="0dec7-1245">AKS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1245">AKS</span></span>

* <span data-ttu-id="0dec7-1246">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1246">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1247">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1247">Batch</span></span>

* <span data-ttu-id="0dec7-1248">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="0dec7-1248">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-1249">IOT</span><span class="sxs-lookup"><span data-stu-id="0dec7-1249">IOT</span></span>

* <span data-ttu-id="0dec7-1250">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1250">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1251">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1251">Network</span></span>

* <span data-ttu-id="0dec7-1252">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1252">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0dec7-1253">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0dec7-1253">Policy Insights</span></span>

* <span data-ttu-id="0dec7-1254">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1254">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="0dec7-1255">ARM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1255">ARM</span></span>

* <span data-ttu-id="0dec7-1256">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1256">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1257">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1257">SQL</span></span>

* <span data-ttu-id="0dec7-1258">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="0dec7-1258">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="0dec7-1259">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1259">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="0dec7-1260">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1260">Storage</span></span>

* <span data-ttu-id="0dec7-1261">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1261">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1262">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1262">VM</span></span>

* <span data-ttu-id="0dec7-1263">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1263">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="0dec7-1264">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1264">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="0dec7-1265">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1265">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="0dec7-1266">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1266">May 22, 2018</span></span>

<span data-ttu-id="0dec7-1267">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="0dec7-1267">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1268">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1268">Core</span></span>

* <span data-ttu-id="0dec7-1269">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1269">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1270">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1270">ACS</span></span>

* <span data-ttu-id="0dec7-1271">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1271">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="0dec7-1272">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1272">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1273">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-1273">AppService</span></span>

* <span data-ttu-id="0dec7-1274">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1274">Improved generic update commands</span></span>
* <span data-ttu-id="0dec7-1275">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1275">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1276">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1276">Container</span></span>

* <span data-ttu-id="0dec7-1277">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1277">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="0dec7-1278">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1278">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1279">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1279">Extension</span></span>

* <span data-ttu-id="0dec7-1280">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1280">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1281">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1281">Interactive</span></span>

* <span data-ttu-id="0dec7-1282">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1282">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="0dec7-1283">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1283">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-1284">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0dec7-1284">KeyVault</span></span>

* <span data-ttu-id="0dec7-1285">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1285">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1286">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1286">Network</span></span>

* <span data-ttu-id="0dec7-1287">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1287">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="0dec7-1288">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1288">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1289">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1289">SQL</span></span>

* <span data-ttu-id="0dec7-1290">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="0dec7-1290">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="0dec7-1291">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="0dec7-1291">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="0dec7-1292">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1292">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="0dec7-1293">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1293">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="0dec7-1294">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1294">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="0dec7-1295">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1295">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="0dec7-1296">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1296">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="0dec7-1297">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1297">`edition`.</span></span> <span data-ttu-id="0dec7-1298">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1298">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="0dec7-1299">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1299">`elasticPoolName`.</span></span> <span data-ttu-id="0dec7-1300">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1300">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="0dec7-1301">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1301">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="0dec7-1302">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1302">`edition`.</span></span> <span data-ttu-id="0dec7-1303">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1303">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="0dec7-1304">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1304">`dtu`.</span></span> <span data-ttu-id="0dec7-1305">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1305">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="0dec7-1306">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1306">`databaseDtuMin`.</span></span> <span data-ttu-id="0dec7-1307">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1307">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="0dec7-1308">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1308">`databaseDtuMax`.</span></span> <span data-ttu-id="0dec7-1309">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1309">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="0dec7-1310">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1310">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="0dec7-1311">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1311">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1312">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1312">Storage</span></span>

* <span data-ttu-id="0dec7-1313">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1313">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="0dec7-1314">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1314">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1315">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1315">VM</span></span>

* <span data-ttu-id="0dec7-1316">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1316">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="0dec7-1317">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1317">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="0dec7-1318">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1318">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="0dec7-1319">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1319">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="0dec7-1320">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1320">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="0dec7-1321">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1321">May 7, 2018</span></span>

<span data-ttu-id="0dec7-1322">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="0dec7-1322">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1323">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1323">Core</span></span>

* <span data-ttu-id="0dec7-1324">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1324">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="0dec7-1325">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1325">Added limited support for positional arguments</span></span>
* <span data-ttu-id="0dec7-1326">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1326">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="0dec7-1327">#5591</span><span class="sxs-lookup"><span data-stu-id="0dec7-1327">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="0dec7-1328">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1328">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="0dec7-1329">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1329">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="0dec7-1330">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1330">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="0dec7-1331">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1331">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="0dec7-1332">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1332">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1333">ACR</span></span>

* <span data-ttu-id="0dec7-1334">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1334">Added ACR Build commands</span></span>
* <span data-ttu-id="0dec7-1335">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1335">Improved resource not found error messages</span></span>
* <span data-ttu-id="0dec7-1336">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1336">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="0dec7-1337">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1337">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="0dec7-1338">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1338">Improved repository commands error messages</span></span>
* <span data-ttu-id="0dec7-1339">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1339">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1340">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1340">ACS</span></span>

* <span data-ttu-id="0dec7-1341">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1341">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="0dec7-1342">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1342">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="0dec7-1343">AMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1343">AMS</span></span>

* <span data-ttu-id="0dec7-1344">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="0dec7-1344">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1345">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1345">Appservice</span></span>

* <span data-ttu-id="0dec7-1346">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1346">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="0dec7-1347">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1347">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="0dec7-1348">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1348">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="0dec7-1349">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1349">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0dec7-1350">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1350">Batch AI</span></span>

* <span data-ttu-id="0dec7-1351">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1351">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0dec7-1352">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0dec7-1352">Cognitive Services</span></span>

* <span data-ttu-id="0dec7-1353">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1353">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-1354">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-1354">Consumption</span></span>

* <span data-ttu-id="0dec7-1355">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1355">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1356">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1356">Container</span></span>

* <span data-ttu-id="0dec7-1357">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1357">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0dec7-1358">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0dec7-1358">Cosmos DB</span></span>

* <span data-ttu-id="0dec7-1359">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0dec7-1359">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="0dec7-1360">DMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1360">DMS</span></span>

* <span data-ttu-id="0dec7-1361">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1361">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1362">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1362">Extension</span></span>

* <span data-ttu-id="0dec7-1363">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1363">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1364">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1364">Interactive</span></span>

* <span data-ttu-id="0dec7-1365">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1365">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="0dec7-1366">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="0dec7-1366">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="0dec7-1367">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1367">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="0dec7-1368">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1368">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="0dec7-1369">랩</span><span class="sxs-lookup"><span data-stu-id="0dec7-1369">Lab</span></span>

* <span data-ttu-id="0dec7-1370">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1370">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1371">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1371">Network</span></span>

* <span data-ttu-id="0dec7-1372">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1372">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="0dec7-1373">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1373">Profile</span></span>

* <span data-ttu-id="0dec7-1374">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1374">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="0dec7-1375">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1375">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="0dec7-1376">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1376">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="0dec7-1377">Redis</span><span class="sxs-lookup"><span data-stu-id="0dec7-1377">Redis</span></span>

* <span data-ttu-id="0dec7-1378">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1378">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="0dec7-1379">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1379">Deprecated `redis list-all`.</span></span> <span data-ttu-id="0dec7-1380">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1380">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="0dec7-1381">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1381">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="0dec7-1382">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1382">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1383">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1383">Role</span></span>

* <span data-ttu-id="0dec7-1384">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1384">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1385">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1385">Storage</span></span>

* <span data-ttu-id="0dec7-1386">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1386">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="0dec7-1387">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="0dec7-1387">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="0dec7-1388">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="0dec7-1388">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="0dec7-1389">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1389">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="0dec7-1390">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1390">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1391">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1391">VM</span></span>

* <span data-ttu-id="0dec7-1392">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1392">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="0dec7-1393">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1393">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="0dec7-1394">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="0dec7-1394">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="0dec7-1395">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1395">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="0dec7-1396">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1396">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="0dec7-1397">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1397">Added write accelerator support</span></span>
* <span data-ttu-id="0dec7-1398">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1398">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="0dec7-1399">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1399">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="0dec7-1400">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1400">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="0dec7-1401">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1401">April 10, 2018</span></span>

<span data-ttu-id="0dec7-1402">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="0dec7-1402">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1403">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1403">ACR</span></span>

* <span data-ttu-id="0dec7-1404">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="0dec7-1404">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1405">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1405">ACS</span></span>

* <span data-ttu-id="0dec7-1406">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1406">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1407">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1407">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="0dec7-1409">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1409">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="0dec7-1410">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0dec7-1410">BatchAI</span></span>

* <span data-ttu-id="0dec7-1411">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1411">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="0dec7-1412">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="0dec7-1412">Job level mounting</span></span>
  - <span data-ttu-id="0dec7-1413">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="0dec7-1413">Environment variables with secret values</span></span>
  - <span data-ttu-id="0dec7-1414">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1414">Performance counters settings</span></span>
  - <span data-ttu-id="0dec7-1415">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="0dec7-1415">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="0dec7-1416">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1416">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="0dec7-1417">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="0dec7-1417">Usage and limits reporting</span></span>
  - <span data-ttu-id="0dec7-1418">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1418">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="0dec7-1419">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1419">Support for custom images</span></span>
  - <span data-ttu-id="0dec7-1420">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1420">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="0dec7-1421">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1421">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="0dec7-1422">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1422">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="0dec7-1423">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1423">National clouds are supported</span></span>
* <span data-ttu-id="0dec7-1424">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1424">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="0dec7-1425">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1425">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="0dec7-1426">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1426">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="0dec7-1427">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1427">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="0dec7-1428">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="0dec7-1428">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="0dec7-1429">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="0dec7-1429">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="0dec7-1430">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1430">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="0dec7-1431">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1431">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="0dec7-1432">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1432">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="0dec7-1433">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1433">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="0dec7-1434">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1434">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="0dec7-1435">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1435">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="0dec7-1436">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1436">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="0dec7-1437">결제</span><span class="sxs-lookup"><span data-stu-id="0dec7-1437">Billing</span></span>

* <span data-ttu-id="0dec7-1438">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1438">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-1439">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-1439">Consumption</span></span>

* <span data-ttu-id="0dec7-1440">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1440">Added `marketplace` commands</span></span>
* <span data-ttu-id="0dec7-1441">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1441">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="0dec7-1442">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1442">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="0dec7-1443">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1443">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="0dec7-1444">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1444">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="0dec7-1445">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1445">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1446">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1446">Container</span></span>

* <span data-ttu-id="0dec7-1447">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1447">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="0dec7-1448">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="0dec7-1448">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1449">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1449">Extension</span></span>

* <span data-ttu-id="0dec7-1450">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1450">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1451">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1451">Interactive</span></span>

* <span data-ttu-id="0dec7-1452">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1452">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="0dec7-1453">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1453">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="0dec7-1454">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1454">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1455">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1455">Network</span></span>

* <span data-ttu-id="0dec7-1456">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1456">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="0dec7-1457">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1457">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="0dec7-1458">#4910</span><span class="sxs-lookup"><span data-stu-id="0dec7-1458">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="0dec7-1459">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1459">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="0dec7-1460">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1460">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="0dec7-1461">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1461">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="0dec7-1462">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1462">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="0dec7-1463">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1463">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-1464">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1464">Profile</span></span>

* <span data-ttu-id="0dec7-1465">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1465">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="0dec7-1466">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1466">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-1467">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1467">RDBMS</span></span>

* <span data-ttu-id="0dec7-1468">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1468">Added `georestore` command</span></span>
* <span data-ttu-id="0dec7-1469">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1469">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1470">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1470">Resource</span></span>

* <span data-ttu-id="0dec7-1471">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1471">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="0dec7-1472">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1472">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1473">SQL</span></span>

* <span data-ttu-id="0dec7-1474">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1474">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1475">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1475">Storage</span></span>

* <span data-ttu-id="0dec7-1476">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1476">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1477">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1477">VM</span></span>

* <span data-ttu-id="0dec7-1478">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1478">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="0dec7-1479">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1479">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="0dec7-1481">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1481">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="0dec7-1482">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1482">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="0dec7-1483">#5718</span><span class="sxs-lookup"><span data-stu-id="0dec7-1483">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="0dec7-1484">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1484">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="0dec7-1485">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1485">March 27, 2018</span></span>

<span data-ttu-id="0dec7-1486">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="0dec7-1486">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1487">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1487">Core</span></span>

* <span data-ttu-id="0dec7-1488">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="0dec7-1488">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1489">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1489">ACS</span></span>

* <span data-ttu-id="0dec7-1490">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1490">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1491">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1491">Appservice</span></span>

* <span data-ttu-id="0dec7-1492">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1492">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="0dec7-1493">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1493">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0dec7-1494">Backup</span><span class="sxs-lookup"><span data-stu-id="0dec7-1494">Backup</span></span>

* <span data-ttu-id="0dec7-1495">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1495">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="0dec7-1496">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1496">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="0dec7-1497">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1497">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="0dec7-1498">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1498">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1499">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1499">Container</span></span>

* <span data-ttu-id="0dec7-1500">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1500">Added `container exec` command.</span></span> <span data-ttu-id="0dec7-1501">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1501">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="0dec7-1502">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-1502">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1503">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1503">Extension</span></span>

* <span data-ttu-id="0dec7-1504">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1504">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="0dec7-1505">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1505">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="0dec7-1506">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1506">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1507">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1507">Interactive</span></span>

* <span data-ttu-id="0dec7-1508">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="0dec7-1508">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="0dec7-1509">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1509">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="0dec7-1510">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1510">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="0dec7-1511">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1511">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="0dec7-1512">랩</span><span class="sxs-lookup"><span data-stu-id="0dec7-1512">Lab</span></span>

* <span data-ttu-id="0dec7-1513">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1513">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1514">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1514">Monitor</span></span>

* <span data-ttu-id="0dec7-1515">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1515">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="0dec7-1516">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1516">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="0dec7-1517">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1517">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1518">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1518">Network</span></span>

* <span data-ttu-id="0dec7-1519">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1519">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-1520">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1520">Profile</span></span>

* <span data-ttu-id="0dec7-1521">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1521">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-1522">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1522">RDBMS</span></span>

* <span data-ttu-id="0dec7-1523">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1523">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1524">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1524">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="0dec7-1526">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1526">Role</span></span>

* <span data-ttu-id="0dec7-1527">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1527">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="0dec7-1528">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1528">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="0dec7-1529">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1529">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="0dec7-1530">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1530">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="0dec7-1531">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1531">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1532">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1532">Storage</span></span>

* <span data-ttu-id="0dec7-1533">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1533">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="0dec7-1534">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="0dec7-1534">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1535">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1535">VM</span></span>

* <span data-ttu-id="0dec7-1536">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1536">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="0dec7-1537">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1537">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="0dec7-1538">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1538">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="0dec7-1539">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1539">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="0dec7-1540">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1540">March 13, 2018</span></span>

<span data-ttu-id="0dec7-1541">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="0dec7-1541">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1542">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1542">ACR</span></span>

* <span data-ttu-id="0dec7-1543">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1543">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="0dec7-1544">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1544">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="0dec7-1545">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1545">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1546">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1546">ACS</span></span>

* <span data-ttu-id="0dec7-1547">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1547">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="0dec7-1548">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1548">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="0dec7-1549">Advisor</span><span class="sxs-lookup"><span data-stu-id="0dec7-1549">Advisor</span></span>

* <span data-ttu-id="0dec7-1550">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1550">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="0dec7-1551">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1551">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="0dec7-1552">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1552">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="0dec7-1553">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1553">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="0dec7-1554">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1554">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1555">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1555">Appservice</span></span>

* <span data-ttu-id="0dec7-1556">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1556">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="0dec7-1557">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1557">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0dec7-1558">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0dec7-1558">Eventhubs</span></span>

* <span data-ttu-id="0dec7-1559">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1559">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1560">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1560">Extension</span></span>

* <span data-ttu-id="0dec7-1561">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1561">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1562">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1562">Interactive</span></span>

* <span data-ttu-id="0dec7-1563">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="0dec7-1563">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="0dec7-1564">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="0dec7-1564">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="0dec7-1565">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1565">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="0dec7-1566">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1566">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1567">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1567">Monitor</span></span>

* <span data-ttu-id="0dec7-1568">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1568">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="0dec7-1569">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1569">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="0dec7-1570">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1570">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="0dec7-1571">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1571">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1572">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1572">Network</span></span>

* <span data-ttu-id="0dec7-1573">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1573">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="0dec7-1574">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="0dec7-1574">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="0dec7-1575">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1575">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="0dec7-1576">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1576">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-1577">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1577">Profile</span></span>

* <span data-ttu-id="0dec7-1578">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1578">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="0dec7-1579">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1579">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-1580">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1580">RDBMS</span></span>

* <span data-ttu-id="0dec7-1581">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1581">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="0dec7-1582">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0dec7-1582">Service Bus</span></span>

* <span data-ttu-id="0dec7-1583">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1583">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1584">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1584">Storage</span></span>

* <span data-ttu-id="0dec7-1585">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1585">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="0dec7-1586">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1586">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1587">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1587">VM</span></span>

* <span data-ttu-id="0dec7-1588">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1588">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="0dec7-1589">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-1589">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="0dec7-1590">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1590">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="0dec7-1591">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1591">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="0dec7-1592">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1592">February 27, 2018</span></span>

<span data-ttu-id="0dec7-1593">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="0dec7-1593">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1594">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1594">Core</span></span>

* <span data-ttu-id="0dec7-1595">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="0dec7-1595">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="0dec7-1596">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1596">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="0dec7-1597">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1597">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1598">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1598">ACS</span></span>

* <span data-ttu-id="0dec7-1599">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1599">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="0dec7-1600">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1600">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="0dec7-1601">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1601">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="0dec7-1602">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1602">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1603">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1603">Appservice</span></span>

* <span data-ttu-id="0dec7-1604">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="0dec7-1604">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="0dec7-1605">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1605">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0dec7-1606">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0dec7-1606">Cognitive Services</span></span>

* <span data-ttu-id="0dec7-1607">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1607">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-1608">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-1608">Consumption</span></span>

* <span data-ttu-id="0dec7-1609">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1609">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="0dec7-1610">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1610">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1611">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1611">Container</span></span>

* <span data-ttu-id="0dec7-1612">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1612">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1613">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1613">Network</span></span>

* <span data-ttu-id="0dec7-1614">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1614">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1615">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1615">Resource</span></span>

* <span data-ttu-id="0dec7-1616">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1616">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1617">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1617">Role</span></span>

* <span data-ttu-id="0dec7-1618">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1618">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1619">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1619">SQL</span></span>

* <span data-ttu-id="0dec7-1620">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1620">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1621">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1621">Storage</span></span>

* <span data-ttu-id="0dec7-1622">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1622">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1623">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1623">VM</span></span>

* <span data-ttu-id="0dec7-1624">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1624">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="0dec7-1625">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1625">February 13, 2018</span></span>

<span data-ttu-id="0dec7-1626">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="0dec7-1626">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1627">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1627">Core</span></span>

* <span data-ttu-id="0dec7-1628">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1628">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1629">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1629">ACS</span></span>

* <span data-ttu-id="0dec7-1630">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1630">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="0dec7-1631">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1631">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="0dec7-1632">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1632">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="0dec7-1633">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="0dec7-1633">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="0dec7-1634">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1634">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="0dec7-1635">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-1635">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="0dec7-1636">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1636">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="0dec7-1637">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1637">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1638">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1638">Appservice</span></span>

* <span data-ttu-id="0dec7-1639">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1639">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="0dec7-1640">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1640">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-1641">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-1641">CDN</span></span>

* <span data-ttu-id="0dec7-1642">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1642">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1643">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1643">Container</span></span>

* <span data-ttu-id="0dec7-1644">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1644">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="0dec7-1645">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1645">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-1646">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-1646">CosmosDB</span></span>

* <span data-ttu-id="0dec7-1647">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1647">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1648">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1648">Extension</span></span>

* <span data-ttu-id="0dec7-1649">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1649">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="0dec7-1650">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1650">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="0dec7-1651">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="0dec7-1651">Feedback</span></span>

* <span data-ttu-id="0dec7-1652">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1652">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1653">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1653">Interactive</span></span>

* <span data-ttu-id="0dec7-1654">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1654">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="0dec7-1655">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1655">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-1656">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-1656">IoT</span></span>

* <span data-ttu-id="0dec7-1657">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1657">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0dec7-1658">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1658">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0dec7-1659">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1659">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="0dec7-1660">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1660">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1661">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1661">Monitor</span></span>

* <span data-ttu-id="0dec7-1662">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1662">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1663">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1663">Network</span></span>

* <span data-ttu-id="0dec7-1664">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1664">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="0dec7-1665">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1665">Profile</span></span>

* <span data-ttu-id="0dec7-1666">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1666">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1667">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1667">Resource</span></span>

* <span data-ttu-id="0dec7-1668">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1668">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1669">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1669">Role</span></span>

* <span data-ttu-id="0dec7-1670">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1670">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1671">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1671">SQL</span></span>

* <span data-ttu-id="0dec7-1672">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1672">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="0dec7-1673">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1673">Added `sql db rename`</span></span>
* <span data-ttu-id="0dec7-1674">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1674">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1675">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1675">Storage</span></span>

* <span data-ttu-id="0dec7-1676">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1676">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1677">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1677">VM</span></span>

* <span data-ttu-id="0dec7-1678">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1678">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="0dec7-1679">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1679">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="0dec7-1680">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1680">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="0dec7-1681">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1681">January 31, 2018</span></span>

<span data-ttu-id="0dec7-1682">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="0dec7-1682">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1683">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1683">Core</span></span>

* <span data-ttu-id="0dec7-1684">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1684">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="0dec7-1685">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1685">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="0dec7-1686">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1686">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="0dec7-1687">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="0dec7-1687">Use `--verbose` to see</span></span>
* <span data-ttu-id="0dec7-1688">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1688">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1689">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1689">ACS</span></span>

* <span data-ttu-id="0dec7-1690">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1690">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="0dec7-1691">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="0dec7-1691">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1692">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1692">Appservice</span></span>

* <span data-ttu-id="0dec7-1693">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1693">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="0dec7-1694">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-1694">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-1695">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-1695">CDN</span></span>

* <span data-ttu-id="0dec7-1696">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1696">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-1697">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-1697">CosmosDB</span></span>

* <span data-ttu-id="0dec7-1698">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1698">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1699">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1699">Interactive</span></span>

* <span data-ttu-id="0dec7-1700">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1700">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1701">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1701">Network</span></span>

* <span data-ttu-id="0dec7-1702">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1702">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="0dec7-1703">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1703">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="0dec7-1704">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1704">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="0dec7-1705">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1705">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="0dec7-1706">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1706">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="0dec7-1707">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="0dec7-1707">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="0dec7-1708">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1708">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="0dec7-1709">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1709">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="0dec7-1710">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1710">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="0dec7-1711">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1711">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-1712">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1712">Profile</span></span>

* <span data-ttu-id="0dec7-1713">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1713">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1714">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1714">Resource</span></span>

* <span data-ttu-id="0dec7-1715">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1715">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1716">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1716">Storage</span></span>

* <span data-ttu-id="0dec7-1717">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1717">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="0dec7-1718">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1718">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="0dec7-1719">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1719">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="0dec7-1720">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1720">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="0dec7-1721">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1721">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1722">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1722">VM</span></span>

* <span data-ttu-id="0dec7-1723">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1723">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="0dec7-1724">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1724">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="0dec7-1725">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1725">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="0dec7-1726">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1726">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="0dec7-1727">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1727">January 17, 2018</span></span>

<span data-ttu-id="0dec7-1728">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="0dec7-1728">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1729">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1729">ACR</span></span>

* <span data-ttu-id="0dec7-1730">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1730">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="0dec7-1731">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1731">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1732">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1732">ACS</span></span>

* <span data-ttu-id="0dec7-1733">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1733">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="0dec7-1734">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1734">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1735">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1735">Appservice</span></span>

* <span data-ttu-id="0dec7-1736">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1736">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="0dec7-1737">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1737">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="0dec7-1738">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1738">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="0dec7-1739">Backup</span><span class="sxs-lookup"><span data-stu-id="0dec7-1739">Backup</span></span>

* <span data-ttu-id="0dec7-1740">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1740">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="0dec7-1741">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1741">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="0dec7-1742">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1742">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="0dec7-1743">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1743">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="0dec7-1744">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1744">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1745">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1745">Batch</span></span>

* <span data-ttu-id="0dec7-1746">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1746">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="0dec7-1747">클라우드</span><span class="sxs-lookup"><span data-stu-id="0dec7-1747">Cloud</span></span>

* <span data-ttu-id="0dec7-1748">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1748">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-1749">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-1749">Consumption</span></span>

* <span data-ttu-id="0dec7-1750">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1750">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="0dec7-1751">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0dec7-1751">Event Grid</span></span>

* <span data-ttu-id="0dec7-1752">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1752">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0dec7-1753">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1753">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0dec7-1754">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1754">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="0dec7-1755">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1755">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="0dec7-1756">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1756">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="0dec7-1757">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1757">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="0dec7-1758">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1758">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="0dec7-1759">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1759">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-1760">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-1760">Interactive</span></span>

* <span data-ttu-id="0dec7-1761">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1761">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="0dec7-1762">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1762">Fixed errors on startup</span></span>
* <span data-ttu-id="0dec7-1763">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1763">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-1764">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-1764">IoT</span></span>

* <span data-ttu-id="0dec7-1765">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1765">Added support for device provisioning service</span></span>
* <span data-ttu-id="0dec7-1766">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1766">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="0dec7-1767">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1767">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1768">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1768">Monitor</span></span>

* <span data-ttu-id="0dec7-1769">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1769">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="0dec7-1770">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="0dec7-1770">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="0dec7-1771">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1771">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1772">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1772">Network</span></span>

* <span data-ttu-id="0dec7-1773">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1773">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="0dec7-1774">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1774">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-1775">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-1775">Profile</span></span>

* <span data-ttu-id="0dec7-1776">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1776">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1777">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1777">Role</span></span>

* <span data-ttu-id="0dec7-1778">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1778">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0dec7-1779">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0dec7-1779">Service Fabric</span></span>

* <span data-ttu-id="0dec7-1780">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1780">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="0dec7-1781">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1781">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1782">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1782">VM</span></span>

* <span data-ttu-id="0dec7-1783">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-1783">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="0dec7-1784">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1784">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="0dec7-1785">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1785">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="0dec7-1786">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1786">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="0dec7-1787">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1787">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="0dec7-1788">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1788">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0dec7-1789">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1789">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="0dec7-1790">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1790">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="0dec7-1791">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1791">December 19, 2017</span></span>

<span data-ttu-id="0dec7-1792">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="0dec7-1792">Version 2.0.23</span></span>

* <span data-ttu-id="0dec7-1793">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1793">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1794">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1794">Container</span></span>

* <span data-ttu-id="0dec7-1795">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1795">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1796">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1796">Network</span></span>

* <span data-ttu-id="0dec7-1797">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1797">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="0dec7-1798">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1798">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1799">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1799">Storage</span></span>

* <span data-ttu-id="0dec7-1800">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1800">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1801">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1801">VM</span></span>

* <span data-ttu-id="0dec7-1802">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1802">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="0dec7-1803">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1803">December 5, 2017</span></span>

<span data-ttu-id="0dec7-1804">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="0dec7-1804">Version 2.0.22</span></span>

* <span data-ttu-id="0dec7-1805">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1805">Removed `az component` commands.</span></span> <span data-ttu-id="0dec7-1806">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1806">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1807">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1807">Core</span></span>
* <span data-ttu-id="0dec7-1808">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1808">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="0dec7-1809">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1809">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1810">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1810">ACS</span></span>

* <span data-ttu-id="0dec7-1811">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1811">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="0dec7-1812">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1812">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="0dec7-1813">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1813">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="0dec7-1814">Advisor</span><span class="sxs-lookup"><span data-stu-id="0dec7-1814">Advisor</span></span>

* <span data-ttu-id="0dec7-1815">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1815">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1816">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1816">Appservice</span></span>

* <span data-ttu-id="0dec7-1817">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1817">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="0dec7-1818">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1818">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="0dec7-1819">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1819">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="0dec7-1820">Consumption</span><span class="sxs-lookup"><span data-stu-id="0dec7-1820">Consumption</span></span>

* <span data-ttu-id="0dec7-1821">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1821">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1822">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1822">Container</span></span>

* <span data-ttu-id="0dec7-1823">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1823">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1824">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1824">Monitor</span></span>

* <span data-ttu-id="0dec7-1825">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1825">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1826">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1826">Resource</span></span>

* <span data-ttu-id="0dec7-1827">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1827">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-1828">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-1828">Role</span></span>

* <span data-ttu-id="0dec7-1829">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1829">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="0dec7-1830">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1830">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="0dec7-1831">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1831">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1832">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1832">SQL</span></span>

* <span data-ttu-id="0dec7-1833">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1833">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="0dec7-1834">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1834">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1835">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1835">VM</span></span>

* <span data-ttu-id="0dec7-1836">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1836">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="0dec7-1837">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1837">November 14, 2017</span></span>

<span data-ttu-id="0dec7-1838">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="0dec7-1838">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1839">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1839">ACR</span></span>

* <span data-ttu-id="0dec7-1840">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1840">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="0dec7-1841">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1841">ACS</span></span>

* <span data-ttu-id="0dec7-1842">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1842">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="0dec7-1843">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="0dec7-1843">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="0dec7-1844">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1844">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="0dec7-1845">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1845">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="0dec7-1846">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1846">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1847">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1847">Appservice</span></span>

* <span data-ttu-id="0dec7-1848">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1848">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="0dec7-1849">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1849">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="0dec7-1850">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1850">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="0dec7-1851">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1851">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="0dec7-1852">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1852">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="0dec7-1853">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="0dec7-1853">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1854">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1854">Batch</span></span>

* <span data-ttu-id="0dec7-1855">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1855">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="0dec7-1856">Batchai</span><span class="sxs-lookup"><span data-stu-id="0dec7-1856">Batchai</span></span>

* <span data-ttu-id="0dec7-1857">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1857">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="0dec7-1858">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1858">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="0dec7-1859">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1859">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="0dec7-1860">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1860">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="0dec7-1861">클라우드</span><span class="sxs-lookup"><span data-stu-id="0dec7-1861">Cloud</span></span>

* <span data-ttu-id="0dec7-1862">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1862">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-1863">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-1863">Container</span></span>

* <span data-ttu-id="0dec7-1864">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1864">Added support to open multiple ports</span></span>
* <span data-ttu-id="0dec7-1865">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1865">Added container group restart policy</span></span>
* <span data-ttu-id="0dec7-1866">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1866">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="0dec7-1867">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="0dec7-1867">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0dec7-1868">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0dec7-1868">Data Lake Analytics</span></span>

* <span data-ttu-id="0dec7-1869">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1869">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0dec7-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0dec7-1870">Data Lake Store</span></span>

* <span data-ttu-id="0dec7-1871">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1871">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-1872">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-1872">Extension</span></span>

* <span data-ttu-id="0dec7-1873">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1873">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="0dec7-1874">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1874">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-1875">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-1875">IoT</span></span>

* <span data-ttu-id="0dec7-1876">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1876">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1877">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1877">Monitor</span></span>

* <span data-ttu-id="0dec7-1878">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1878">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1879">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1879">Network</span></span>

* <span data-ttu-id="0dec7-1880">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1880">Added support for CAA DNS records</span></span>
* <span data-ttu-id="0dec7-1881">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1881">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="0dec7-1882">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1882">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="0dec7-1883">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1883">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="0dec7-1884">예약</span><span class="sxs-lookup"><span data-stu-id="0dec7-1884">Reservations</span></span>

* <span data-ttu-id="0dec7-1885">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1885">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1886">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1886">Resource</span></span>

* <span data-ttu-id="0dec7-1887">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1887">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1888">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1888">SQL</span></span>

* <span data-ttu-id="0dec7-1889">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1889">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1890">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1890">Storage</span></span>

* <span data-ttu-id="0dec7-1891">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-1891">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="0dec7-1892">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1892">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="0dec7-1893">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1893">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="0dec7-1894">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="0dec7-1894">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="0dec7-1895">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1895">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="0dec7-1896">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1896">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="0dec7-1897">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1897">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1898">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1898">VM</span></span>

* <span data-ttu-id="0dec7-1899">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1899">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="0dec7-1900">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1900">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="0dec7-1901">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1901">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="0dec7-1902">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1902">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="0dec7-1903">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1903">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="0dec7-1904">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1904">October 24, 2017</span></span>

<span data-ttu-id="0dec7-1905">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="0dec7-1905">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1906">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1906">Core</span></span>

* <span data-ttu-id="0dec7-1907">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1907">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-1908">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-1908">ACR</span></span>

* <span data-ttu-id="0dec7-1909">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1909">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="0dec7-1910">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1910">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="0dec7-1911">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="0dec7-1911">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1912">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1912">ACS</span></span>

* <span data-ttu-id="0dec7-1913">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1913">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="0dec7-1914">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1914">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1915">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1915">Appservice</span></span>

* <span data-ttu-id="0dec7-1916">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1916">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="0dec7-1917">구성 요소</span><span class="sxs-lookup"><span data-stu-id="0dec7-1917">Component</span></span>

* <span data-ttu-id="0dec7-1918">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1918">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-1919">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-1919">Monitor</span></span>

* <span data-ttu-id="0dec7-1920">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1920">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1921">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1921">Resource</span></span>

* <span data-ttu-id="0dec7-1922">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1922">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="0dec7-1923">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-1923">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1924">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1924">VM</span></span>

* <span data-ttu-id="0dec7-1925">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1925">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="0dec7-1926">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1926">October 9, 2017</span></span>

<span data-ttu-id="0dec7-1927">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="0dec7-1927">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-1928">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-1928">Core</span></span>

* <span data-ttu-id="0dec7-1929">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1929">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1930">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1930">Appservice</span></span>

* <span data-ttu-id="0dec7-1931">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1931">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-1932">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-1932">Batch</span></span>

* <span data-ttu-id="0dec7-1933">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1933">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="0dec7-1934">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1934">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="0dec7-1935">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1935">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="0dec7-1936">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1936">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="0dec7-1937">Batchai</span><span class="sxs-lookup"><span data-stu-id="0dec7-1937">Batchai</span></span>

* <span data-ttu-id="0dec7-1938">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1938">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-1939">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0dec7-1939">Keyvault</span></span>

* <span data-ttu-id="0dec7-1940">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1940">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="0dec7-1941">(#4448)</span><span class="sxs-lookup"><span data-stu-id="0dec7-1941">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="0dec7-1942">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1942">Network</span></span>

* <span data-ttu-id="0dec7-1943">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1943">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="0dec7-1944">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1944">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1945">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1945">Resource</span></span>

* <span data-ttu-id="0dec7-1946">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1946">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="0dec7-1947">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1947">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="0dec7-1948">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1948">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="0dec7-1949">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1949">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1950">Sql</span><span class="sxs-lookup"><span data-stu-id="0dec7-1950">Sql</span></span>

* <span data-ttu-id="0dec7-1951">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1951">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="0dec7-1952">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1952">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="0dec7-1953">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1953">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1954">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1954">Storage</span></span>

* <span data-ttu-id="0dec7-1955">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1955">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1956">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1956">Vm</span></span>

* <span data-ttu-id="0dec7-1957">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1957">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="0dec7-1958">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1958">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="0dec7-1959">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1959">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="0dec7-1960">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1960">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="0dec7-1961">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1961">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="0dec7-1962">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="0dec7-1962">September 22, 2017</span></span>

<span data-ttu-id="0dec7-1963">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="0dec7-1963">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-1964">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1964">Resource</span></span>

* <span data-ttu-id="0dec7-1965">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1965">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="0dec7-1966">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1966">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="0dec7-1967">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1967">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="0dec7-1968">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1968">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-1969">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-1969">Network</span></span>

* <span data-ttu-id="0dec7-1970">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1970">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="0dec7-1971">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1971">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="0dec7-1972">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1972">Added `asg` application security group commands</span></span>
* <span data-ttu-id="0dec7-1973">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1973">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="0dec7-1974">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1974">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0dec7-1975">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1975">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="0dec7-1976">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1976">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-1977">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-1977">Storage</span></span>

* <span data-ttu-id="0dec7-1978">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1978">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0dec7-1979">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0dec7-1979">Eventgrid</span></span>

* <span data-ttu-id="0dec7-1980">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="0dec7-1980">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-1981">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-1981">SQL</span></span>

* <span data-ttu-id="0dec7-1982">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-1982">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="0dec7-1983">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-1983">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="0dec7-1984">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1984">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-1985">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0dec7-1985">Keyvault</span></span>

* <span data-ttu-id="0dec7-1986">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1986">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-1987">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-1987">VM</span></span>

* <span data-ttu-id="0dec7-1988">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1988">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="0dec7-1989">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0dec7-1989">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="0dec7-1990">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1990">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="0dec7-1991">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1991">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="0dec7-1992">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1992">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="0dec7-1993">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1993">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-1994">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-1994">ACS</span></span>

* <span data-ttu-id="0dec7-1995">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1995">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-1996">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-1996">Appservice</span></span>

* <span data-ttu-id="0dec7-1997">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-1997">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0dec7-1998">Backup</span><span class="sxs-lookup"><span data-stu-id="0dec7-1998">Backup</span></span>

* <span data-ttu-id="0dec7-1999">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-1999">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="0dec7-2000">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2000">September 11, 2017</span></span>

<span data-ttu-id="0dec7-2001">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0dec7-2001">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0dec7-2002">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-2002">Core</span></span>

* <span data-ttu-id="0dec7-2003">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2003">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0dec7-2004">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2004">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2005">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2005">Acs</span></span>

* <span data-ttu-id="0dec7-2006">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2006">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0dec7-2007">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2007">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2008">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-2008">Appservice</span></span>

* <span data-ttu-id="0dec7-2009">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2009">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-2010">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-2010">CDN</span></span>

* <span data-ttu-id="0dec7-2011">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2011">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="0dec7-2012">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0dec7-2012">Extension</span></span>

* <span data-ttu-id="0dec7-2013">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2013">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-2014">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0dec7-2014">Keyvault</span></span>

* <span data-ttu-id="0dec7-2015">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2015">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-2016">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-2016">Network</span></span>

* <span data-ttu-id="0dec7-2017">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2017">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0dec7-2018">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-2018">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0dec7-2019">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2019">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0dec7-2020">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2020">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0dec7-2021">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2021">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-2022">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2022">Resource</span></span>

* <span data-ttu-id="0dec7-2023">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2023">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0dec7-2024">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2024">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0dec7-2025">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2025">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0dec7-2026">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="0dec7-2026">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-2027">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-2027">SQL</span></span>

* <span data-ttu-id="0dec7-2028">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2028">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2029">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2029">VM</span></span>

* <span data-ttu-id="0dec7-2030">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2030">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0dec7-2031">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2031">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0dec7-2032">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2032">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0dec7-2033">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2033">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0dec7-2034">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2034">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0dec7-2035">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2035">August 31, 2017</span></span>

<span data-ttu-id="0dec7-2036">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0dec7-2036">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-2037">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0dec7-2037">Keyvault</span></span>

* <span data-ttu-id="0dec7-2038">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2038">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0dec7-2039">Sf</span><span class="sxs-lookup"><span data-stu-id="0dec7-2039">Sf</span></span>

* <span data-ttu-id="0dec7-2040">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2040">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-2041">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2041">Storage</span></span>

* <span data-ttu-id="0dec7-2042">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2042">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0dec7-2043">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2043">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0dec7-2044">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2044">August 28, 2017</span></span>

<span data-ttu-id="0dec7-2045">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0dec7-2045">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0dec7-2046">CLI</span><span class="sxs-lookup"><span data-stu-id="0dec7-2046">CLI</span></span>

* <span data-ttu-id="0dec7-2047">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2047">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2048">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2048">ACS</span></span>

* <span data-ttu-id="0dec7-2049">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2049">Corrected preview regions</span></span>
* <span data-ttu-id="0dec7-2050">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2050">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="0dec7-2051">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2051">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2052">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-2052">Appservice</span></span>

* <span data-ttu-id="0dec7-2053">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2053">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0dec7-2054">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2054">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0dec7-2055">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2055">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0dec7-2056">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2056">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0dec7-2057">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2057">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-2058">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-2058">IoT</span></span>

* <span data-ttu-id="0dec7-2059">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2059">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-2060">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-2060">Network</span></span>

* <span data-ttu-id="0dec7-2061">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2061">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0dec7-2062">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2062">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0dec7-2063">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2063">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0dec7-2064">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2064">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0dec7-2065">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2065">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-2066">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-2066">Profile</span></span>

* <span data-ttu-id="0dec7-2067">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2067">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0dec7-2068">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0dec7-2068">Service Fabric</span></span>

* <span data-ttu-id="0dec7-2069">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2069">Preview release</span></span>
* <span data-ttu-id="0dec7-2070">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2070">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0dec7-2071">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2071">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0dec7-2072">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2072">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-2073">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2073">Storage</span></span>

* <span data-ttu-id="0dec7-2074">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2074">Enabled setting blob tier</span></span>
* <span data-ttu-id="0dec7-2075">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2075">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0dec7-2076">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2076">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="0dec7-2077">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2077">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0dec7-2078">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2078">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0dec7-2079">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2079">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2080">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2080">VM</span></span>

* <span data-ttu-id="0dec7-2081">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2081">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0dec7-2082">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2082">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="0dec7-2083">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2083">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="0dec7-2084">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2084">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0dec7-2085">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2085">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0dec7-2086">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2086">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0dec7-2087">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2087">August 15, 2017</span></span>

<span data-ttu-id="0dec7-2088">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0dec7-2088">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2089">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2089">ACS</span></span>

* <span data-ttu-id="0dec7-2090">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2090">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2091">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-2091">Appservice</span></span>

* <span data-ttu-id="0dec7-2092">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2092">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0dec7-2093">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0dec7-2093">Event Grid</span></span>

* <span data-ttu-id="0dec7-2094">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2094">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0dec7-2095">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2095">August 11, 2017</span></span>

<span data-ttu-id="0dec7-2096">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0dec7-2096">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2097">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2097">ACS</span></span>

* <span data-ttu-id="0dec7-2098">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2098">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-2099">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-2099">Batch</span></span>

* <span data-ttu-id="0dec7-2100">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2100">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0dec7-2101">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2101">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0dec7-2102">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2102">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0dec7-2103">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2103">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0dec7-2104">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2104">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0dec7-2105">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2105">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0dec7-2106">구성 요소</span><span class="sxs-lookup"><span data-stu-id="0dec7-2106">Component</span></span>

* <span data-ttu-id="0dec7-2107">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2107">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0dec7-2108">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0dec7-2108">Container</span></span>

* <span data-ttu-id="0dec7-2109">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2109">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0dec7-2110">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0dec7-2110">Data Lake Store</span></span>

* <span data-ttu-id="0dec7-2111">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2111">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0dec7-2112">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0dec7-2112">Event Grid</span></span>

* <span data-ttu-id="0dec7-2113">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2113">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-2114">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-2114">Network</span></span>

* <span data-ttu-id="0dec7-2115">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2115">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0dec7-2116">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2116">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0dec7-2117">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2117">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0dec7-2118">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2118">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-2119">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-2119">Profile</span></span>

* <span data-ttu-id="0dec7-2120">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2120">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-2121">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2121">Storage</span></span>

* <span data-ttu-id="0dec7-2122">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2122">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2123">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2123">VM</span></span>

* <span data-ttu-id="0dec7-2124">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2124">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0dec7-2125">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2125">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0dec7-2126">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2126">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0dec7-2127">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2127">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0dec7-2128">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2128">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0dec7-2129">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2129">July 28, 2017</span></span>

<span data-ttu-id="0dec7-2130">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0dec7-2130">Version 2.0.12</span></span>

* <span data-ttu-id="0dec7-2131">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2131">Added container commands</span></span>
* <span data-ttu-id="0dec7-2132">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2132">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="0dec7-2133">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-2133">Core</span></span>

* <span data-ttu-id="0dec7-2134">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2134">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0dec7-2135">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2135">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0dec7-2136">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2136">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0dec7-2137">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2137">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0dec7-2138">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="0dec7-2138">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0dec7-2139">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2139">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0dec7-2140">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2140">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0dec7-2141">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2141">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0dec7-2142">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2142">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0dec7-2143">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2143">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0dec7-2144">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="0dec7-2144">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0dec7-2145">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2145">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0dec7-2146">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2146">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0dec7-2147">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2147">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0dec7-2148">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2148">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0dec7-2149">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2149">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0dec7-2150">ACR</span><span class="sxs-lookup"><span data-stu-id="0dec7-2150">ACR</span></span>

* <span data-ttu-id="0dec7-2151">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2151">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0dec7-2152">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2152">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0dec7-2153">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2153">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0dec7-2154">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2154">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0dec7-2155">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2155">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0dec7-2156">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2156">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2157">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2157">ACS</span></span>

* <span data-ttu-id="0dec7-2158">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2158">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2159">App Service</span><span class="sxs-lookup"><span data-stu-id="0dec7-2159">Appservice</span></span>

* <span data-ttu-id="0dec7-2160">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2160">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0dec7-2161">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2161">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0dec7-2162">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2162">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0dec7-2163">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2163">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0dec7-2164">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2164">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0dec7-2165">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2165">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0dec7-2166">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2166">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0dec7-2167">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2167">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0dec7-2168">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2168">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0dec7-2169">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2169">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0dec7-2170">Batch</span><span class="sxs-lookup"><span data-stu-id="0dec7-2170">Batch</span></span>

* <span data-ttu-id="0dec7-2171">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2171">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0dec7-2172">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2172">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0dec7-2173">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2173">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0dec7-2174">CDN</span><span class="sxs-lookup"><span data-stu-id="0dec7-2174">CDN</span></span>

* <span data-ttu-id="0dec7-2175">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2175">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="0dec7-2176">클라우드</span><span class="sxs-lookup"><span data-stu-id="0dec7-2176">Cloud</span></span>

* <span data-ttu-id="0dec7-2177">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2177">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0dec7-2178">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2178">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0dec7-2179">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2179">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0dec7-2180">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2180">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0dec7-2181">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2181">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-2182">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-2182">CosmosDB</span></span>

* <span data-ttu-id="0dec7-2183">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2183">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0dec7-2184">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2184">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0dec7-2185">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0dec7-2185">Data Lake Analytics</span></span>

* <span data-ttu-id="0dec7-2186">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2186">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0dec7-2187">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2187">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0dec7-2188">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2188">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0dec7-2189">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0dec7-2189">Data Lake Store</span></span>

* <span data-ttu-id="0dec7-2190">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2190">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0dec7-2191">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2191">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0dec7-2192">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2192">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0dec7-2193">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="0dec7-2193">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0dec7-2194">대화형</span><span class="sxs-lookup"><span data-stu-id="0dec7-2194">Interactive</span></span>

* <span data-ttu-id="0dec7-2195">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2195">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0dec7-2196">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2196">Increased test coverage</span></span>
* <span data-ttu-id="0dec7-2197">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2197">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0dec7-2198">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2198">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0dec7-2199">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2199">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0dec7-2200">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2200">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0dec7-2201">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2201">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0dec7-2202">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2202">Added `--progress` flag</span></span>
* <span data-ttu-id="0dec7-2203">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2203">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0dec7-2204">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2204">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0dec7-2205">IoT</span><span class="sxs-lookup"><span data-stu-id="0dec7-2205">IoT</span></span>

* <span data-ttu-id="0dec7-2206">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2206">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0dec7-2207">(#3934)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2207">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0dec7-2208">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2208">Key vault</span></span>

* <span data-ttu-id="0dec7-2209">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="0dec7-2209">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0dec7-2210">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2210">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0dec7-2211">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2211">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0dec7-2212">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2212">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0dec7-2213">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2213">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0dec7-2214">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2214">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0dec7-2215">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2215">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0dec7-2216">(#3307)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2216">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0dec7-2217">랩</span><span class="sxs-lookup"><span data-stu-id="0dec7-2217">Lab</span></span>

* <span data-ttu-id="0dec7-2218">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2218">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0dec7-2219">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2219">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-2220">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-2220">Monitor</span></span>

* <span data-ttu-id="0dec7-2221">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2221">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0dec7-2222">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2222">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0dec7-2223">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2223">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0dec7-2224">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2224">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0dec7-2225">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2225">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0dec7-2226">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0dec7-2226">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0dec7-2227">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2227">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0dec7-2228">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2228">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0dec7-2229">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2229">`location` no longer required</span></span>
  * <span data-ttu-id="0dec7-2230">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2230">Add name and ID support for target</span></span>
  * <span data-ttu-id="0dec7-2231">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2231">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0dec7-2232">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2232">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0dec7-2233">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2233">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0dec7-2234">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2234">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0dec7-2235">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2235">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0dec7-2236">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2236">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-2237">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-2237">Network</span></span>

* <span data-ttu-id="0dec7-2238">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2238">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0dec7-2239">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2239">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0dec7-2240">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2240">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0dec7-2241">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2241">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0dec7-2242">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2242">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0dec7-2243">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2243">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0dec7-2244">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2244">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0dec7-2245">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2245">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0dec7-2246">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2246">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0dec7-2247">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2247">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0dec7-2248">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2248">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0dec7-2249">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2249">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0dec7-2250">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2250">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0dec7-2251">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0dec7-2251">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0dec7-2252">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2252">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0dec7-2253">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2253">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0dec7-2254">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2254">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0dec7-2255">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2255">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0dec7-2256">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2256">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0dec7-2257">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2257">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0dec7-2258">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2258">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0dec7-2259">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2259">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0dec7-2260">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2260">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0dec7-2261">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2261">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0dec7-2262">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2262">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0dec7-2263">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2263">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0dec7-2264">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2264">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-2265">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-2265">Profile</span></span>

* <span data-ttu-id="0dec7-2266">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2266">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0dec7-2267">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2267">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0dec7-2268">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2268">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0dec7-2269">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2269">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0dec7-2270">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2270">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0dec7-2271">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2271">RDBMS</span></span>

* <span data-ttu-id="0dec7-2272">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2272">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0dec7-2273">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2273">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0dec7-2274">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2274">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0dec7-2275">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2275">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-2276">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2276">Resource</span></span>

* <span data-ttu-id="0dec7-2277">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2277">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0dec7-2278">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2278">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0dec7-2279">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2279">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0dec7-2280">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2280">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0dec7-2281">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2281">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0dec7-2282">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2282">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0dec7-2283">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2283">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0dec7-2284">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2284">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-2285">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-2285">Role</span></span>

* <span data-ttu-id="0dec7-2286">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2286">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0dec7-2287">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2287">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0dec7-2288">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2288">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0dec7-2289">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2289">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0dec7-2290">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2290">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0dec7-2291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0dec7-2291">Service Fabric</span></span>
* <span data-ttu-id="0dec7-2292">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="0dec7-2292">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0dec7-2293">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2293">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0dec7-2294">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2294">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-2295">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-2295">SQL</span></span>

* <span data-ttu-id="0dec7-2296">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2296">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0dec7-2297">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2297">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0dec7-2298">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2298">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-2299">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2299">Storage</span></span>

* <span data-ttu-id="0dec7-2300">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2300">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0dec7-2301">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2301">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0dec7-2302">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2302">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0dec7-2303">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2303">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="0dec7-2304">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2304">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="0dec7-2305">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2305">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2306">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2306">VM</span></span>

* <span data-ttu-id="0dec7-2307">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2307">Support configuring nsg</span></span>
* <span data-ttu-id="0dec7-2308">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2308">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0dec7-2309">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2309">Support managed service identities</span></span>
* <span data-ttu-id="0dec7-2310">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2310">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="0dec7-2311">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2311">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0dec7-2312">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2312">May 10, 2017</span></span>

<span data-ttu-id="0dec7-2313">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0dec7-2313">Version 2.0.6</span></span>

* <span data-ttu-id="0dec7-2314">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="0dec7-2314">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0dec7-2315">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2315">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0dec7-2316">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2316">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="0dec7-2317">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2317">Include Cognitive Services module</span></span>
* <span data-ttu-id="0dec7-2318">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2318">Include Service Fabric module</span></span>
* <span data-ttu-id="0dec7-2319">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="0dec7-2319">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="0dec7-2320">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2320">Add support for CDN commands</span></span>
* <span data-ttu-id="0dec7-2321">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-2321">Remove Container module</span></span>
* <span data-ttu-id="0dec7-2322">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2322">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0dec7-2323">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2323">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="0dec7-2324">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-2324">Core</span></span>

* <span data-ttu-id="0dec7-2325">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="0dec7-2325">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="0dec7-2326">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2326">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0dec7-2327">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2327">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0dec7-2328">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2328">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0dec7-2329">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2329">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0dec7-2330">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2330">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0dec7-2331">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2331">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0dec7-2332">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2332">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0dec7-2333">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2333">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0dec7-2334">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="0dec7-2334">core: Improved performance</span></span>
* <span data-ttu-id="0dec7-2335">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2335">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0dec7-2336">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2336">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2337">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2337">ACS</span></span>

* <span data-ttu-id="0dec7-2338">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2338">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0dec7-2339">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="0dec7-2339">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0dec7-2340">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="0dec7-2340">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0dec7-2341">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2341">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2342">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-2342">AppService</span></span>

* <span data-ttu-id="0dec7-2343">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2343">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0dec7-2344">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2344">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0dec7-2345">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2345">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0dec7-2346">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="0dec7-2346">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0dec7-2347">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="0dec7-2347">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0dec7-2348">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2348">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0dec7-2349">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2349">support slot swap with preview</span></span>
* <span data-ttu-id="0dec7-2350">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2350">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0dec7-2351">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2351">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0dec7-2352">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-2352">CosmosDB</span></span>

* <span data-ttu-id="0dec7-2353">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="0dec7-2353">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="0dec7-2354">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2354">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0dec7-2355">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2355">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0dec7-2356">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2356">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0dec7-2357">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0dec7-2357">Data Lake Analytics</span></span>

* <span data-ttu-id="0dec7-2358">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2358">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="0dec7-2359">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2359">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0dec7-2360">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2360">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0dec7-2361">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="0dec7-2361">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0dec7-2362">테이블</span><span class="sxs-lookup"><span data-stu-id="0dec7-2362">Table</span></span>
  * <span data-ttu-id="0dec7-2363">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="0dec7-2363">Table valued function</span></span>
  * <span data-ttu-id="0dec7-2364">보기</span><span class="sxs-lookup"><span data-stu-id="0dec7-2364">View</span></span>
  * <span data-ttu-id="0dec7-2365">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2365">Table Statistics.</span></span> <span data-ttu-id="0dec7-2366">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2366">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0dec7-2367">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0dec7-2367">Data Lake Store</span></span>

* <span data-ttu-id="0dec7-2368">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="0dec7-2368">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="0dec7-2369">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2369">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0dec7-2370">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2370">missed help for access show.</span></span> <span data-ttu-id="0dec7-2371">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2371">adding it.</span></span> <span data-ttu-id="0dec7-2372">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2372">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0dec7-2373">찾기</span><span class="sxs-lookup"><span data-stu-id="0dec7-2373">Find</span></span>

* <span data-ttu-id="0dec7-2374">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="0dec7-2374">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0dec7-2375">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0dec7-2375">KeyVault</span></span>

* <span data-ttu-id="0dec7-2376">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2376">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0dec7-2377">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="0dec7-2377">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="0dec7-2378">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2378">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0dec7-2379">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2379">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="0dec7-2380">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2380">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0dec7-2381">랩</span><span class="sxs-lookup"><span data-stu-id="0dec7-2381">Lab</span></span>

* <span data-ttu-id="0dec7-2382">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2382">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="0dec7-2383">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2383">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="0dec7-2384">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="0dec7-2384">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="0dec7-2385">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="0dec7-2385">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="0dec7-2386">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2386">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="0dec7-2387">모니터</span><span class="sxs-lookup"><span data-stu-id="0dec7-2387">Monitor</span></span>

* <span data-ttu-id="0dec7-2388">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2388">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0dec7-2389">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2389">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0dec7-2390">네트워크</span><span class="sxs-lookup"><span data-stu-id="0dec7-2390">Network</span></span>

* <span data-ttu-id="0dec7-2391">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2391">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="0dec7-2392">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2392">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="0dec7-2393">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2393">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="0dec7-2394">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2394">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="0dec7-2395">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2395">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="0dec7-2396">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2396">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="0dec7-2397">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2397">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="0dec7-2398">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2398">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="0dec7-2399">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2399">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="0dec7-2400">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2400">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0dec7-2401">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="0dec7-2401">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="0dec7-2402">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2402">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="0dec7-2403">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2403">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="0dec7-2404">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2404">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="0dec7-2405">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2405">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="0dec7-2406">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2406">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="0dec7-2407">프로필</span><span class="sxs-lookup"><span data-stu-id="0dec7-2407">Profile</span></span>

* <span data-ttu-id="0dec7-2408">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2408">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0dec7-2409">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2409">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0dec7-2410">Redis</span><span class="sxs-lookup"><span data-stu-id="0dec7-2410">Redis</span></span>

* <span data-ttu-id="0dec7-2411">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2411">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0dec7-2412">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="0dec7-2412">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="0dec7-2413">리소스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2413">Resource</span></span>

* <span data-ttu-id="0dec7-2414">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2414">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0dec7-2415">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2415">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0dec7-2416">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2416">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0dec7-2417">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2417">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0dec7-2418">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2418">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0dec7-2419">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2419">Add docs for az lock update.</span></span> <span data-ttu-id="0dec7-2420">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2420">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0dec7-2421">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2421">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0dec7-2422">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2422">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0dec7-2423">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2423">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0dec7-2424">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2424">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0dec7-2425">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2425">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0dec7-2426">역할</span><span class="sxs-lookup"><span data-stu-id="0dec7-2426">Role</span></span>

* <span data-ttu-id="0dec7-2427">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2427">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0dec7-2428">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2428">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0dec7-2429">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2429">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0dec7-2430">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="0dec7-2430">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0dec7-2431">SQL</span><span class="sxs-lookup"><span data-stu-id="0dec7-2431">SQL</span></span>

* <span data-ttu-id="0dec7-2432">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0dec7-2432">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="0dec7-2433">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2433">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0dec7-2434">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2434">Storage</span></span>

* <span data-ttu-id="0dec7-2435">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="0dec7-2435">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="0dec7-2436">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2436">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0dec7-2437">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2437">Add support for large block blob upload</span></span>
* <span data-ttu-id="0dec7-2438">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="0dec7-2438">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2439">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2439">VM</span></span>

* <span data-ttu-id="0dec7-2440">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="0dec7-2440">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0dec7-2441">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2441">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0dec7-2442">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0dec7-2442">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0dec7-2443">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0dec7-2443">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0dec7-2444">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2444">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0dec7-2445">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="0dec7-2445">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0dec7-2446">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2446">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0dec7-2447">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2447">April 3, 2017</span></span>

<span data-ttu-id="0dec7-2448">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0dec7-2448">Version 2.0.2</span></span>

<span data-ttu-id="0dec7-2449">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2449">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="0dec7-2450">코어</span><span class="sxs-lookup"><span data-stu-id="0dec7-2450">Core</span></span>

* <span data-ttu-id="0dec7-2451">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="0dec7-2451">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="0dec7-2452">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2452">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0dec7-2453">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2453">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0dec7-2454">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2454">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0dec7-2455">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2455">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0dec7-2456">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2456">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0dec7-2457">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2457">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0dec7-2458">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2458">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0dec7-2459">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="0dec7-2459">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="0dec7-2460">ACS</span><span class="sxs-lookup"><span data-stu-id="0dec7-2460">ACS</span></span>

* <span data-ttu-id="0dec7-2461">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2461">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0dec7-2462">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2462">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0dec7-2463">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2463">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0dec7-2464">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2464">Add support for windows clusters.</span></span> <span data-ttu-id="0dec7-2465">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2465">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0dec7-2466">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2466">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0dec7-2467">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2467">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="0dec7-2468">AppService</span><span class="sxs-lookup"><span data-stu-id="0dec7-2468">AppService</span></span>

* <span data-ttu-id="0dec7-2469">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2469">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0dec7-2470">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2470">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0dec7-2471">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2471">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0dec7-2472">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2472">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="0dec7-2473">DataLake</span><span class="sxs-lookup"><span data-stu-id="0dec7-2473">DataLake</span></span>

* <span data-ttu-id="0dec7-2474">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2474">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="0dec7-2475">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0dec7-2475">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="0dec7-2476">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="0dec7-2476">DocuemntDB</span></span>

* <span data-ttu-id="0dec7-2477">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2477">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0dec7-2478">VM</span><span class="sxs-lookup"><span data-stu-id="0dec7-2478">VM</span></span>

* <span data-ttu-id="0dec7-2479">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2479">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0dec7-2480">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2480">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0dec7-2481">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2481">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0dec7-2482">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2482">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0dec7-2483">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2483">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0dec7-2484">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2484">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="0dec7-2485">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0dec7-2485">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0dec7-2486">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="0dec7-2486">February 27, 2017</span></span>

<span data-ttu-id="0dec7-2487">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0dec7-2487">Version 2.0.0</span></span>

<span data-ttu-id="0dec7-2488">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2488">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="0dec7-2489">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2489">Container Service (acs)</span></span>
- <span data-ttu-id="0dec7-2490">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="0dec7-2490">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0dec7-2491">네트워킹</span><span class="sxs-lookup"><span data-stu-id="0dec7-2491">Networking</span></span>
- <span data-ttu-id="0dec7-2492">Storage</span><span class="sxs-lookup"><span data-stu-id="0dec7-2492">Storage</span></span>

<span data-ttu-id="0dec7-2493">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2493">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="0dec7-2494">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2494">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="0dec7-2495">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2495">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="0dec7-2496">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2496">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="0dec7-2497">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2497">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="0dec7-2498">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0dec7-2498">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0dec7-2499">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="0dec7-2499">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0dec7-2500">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="0dec7-2500">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="0dec7-2501">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="0dec7-2501">Provide feedback from the command line with the `az feedback` command</span></span>


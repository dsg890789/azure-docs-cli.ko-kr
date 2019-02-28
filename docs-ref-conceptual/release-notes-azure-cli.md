---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158735"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7e14e-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="7e14e-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="7e14e-104">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="7e14e-104">February 12, 2019</span></span>

<span data-ttu-id="7e14e-105">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7e14e-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-106">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-106">Core</span></span>

* <span data-ttu-id="7e14e-107">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7e14e-108">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-109">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-109">ACR</span></span>
* <span data-ttu-id="7e14e-110">[주요 변경 내용] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7e14e-111">[주요 변경 내용] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-112">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-112">ACS</span></span>
* <span data-ttu-id="7e14e-113">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7e14e-114">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7e14e-115">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7e14e-116">AMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-116">AMS</span></span>
* <span data-ttu-id="7e14e-117">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7e14e-118">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-119">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-119">Appservice</span></span>
* <span data-ttu-id="7e14e-120">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7e14e-121">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7e14e-122">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7e14e-123">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7e14e-124">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7e14e-125">Botservice</span><span class="sxs-lookup"><span data-stu-id="7e14e-125">Botservice</span></span>
* <span data-ttu-id="7e14e-126">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7e14e-127">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7e14e-128">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7e14e-129">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7e14e-130">[사용되지 않음] `--proj-name` 인수가 `--proj-file-path`를 위해 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7e14e-131">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7e14e-132">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7e14e-133">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7e14e-134">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7e14e-135">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7e14e-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7e14e-136">Key Vault</span></span>
* <span data-ttu-id="7e14e-137">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-138">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-138">Monitor</span></span>
* <span data-ttu-id="7e14e-139">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-140">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-140">Network</span></span>
* <span data-ttu-id="7e14e-141">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7e14e-142">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7e14e-143">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7e14e-144">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7e14e-145">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="7e14e-145">Policy Insights</span></span>
* <span data-ttu-id="7e14e-146">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-147">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-147">RDBMS</span></span>
* <span data-ttu-id="7e14e-148">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7e14e-149">Redis</span><span class="sxs-lookup"><span data-stu-id="7e14e-149">Redis</span></span>
* <span data-ttu-id="7e14e-150">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7e14e-151">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7e14e-152">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7e14e-153">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7e14e-154">[주요 변경 내용] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7e14e-155">[주요 변경 내용] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7e14e-156">[사용되지 않음] `redis import-method` 명령의 사용 중단에 대한 경고 메시지가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-157">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-157">Role</span></span>
* <span data-ttu-id="7e14e-158">[주요 변경 내용] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7e14e-159">SQL VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-159">SQL VM</span></span>
* <span data-ttu-id="7e14e-160">[사용되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-161">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-161">VM</span></span>
* <span data-ttu-id="7e14e-162">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7e14e-163">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7e14e-164">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7e14e-165">[주요 변경 내용] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7e14e-166">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="7e14e-166">January 31, 2019</span></span>

<span data-ttu-id="7e14e-167">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7e14e-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-168">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-168">Core</span></span>

* <span data-ttu-id="7e14e-169">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7e14e-170">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="7e14e-170">January 28, 2019</span></span>

<span data-ttu-id="7e14e-171">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7e14e-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-172">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-172">ACR</span></span>
* <span data-ttu-id="7e14e-173">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-174">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-174">ACS</span></span>
* <span data-ttu-id="7e14e-175">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7e14e-176">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7e14e-177">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7e14e-178">AMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-178">AMS</span></span>
* <span data-ttu-id="7e14e-179">[주요 변경 내용] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7e14e-180">[주요 변경 내용] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-181">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-181">Appservice</span></span>
* <span data-ttu-id="7e14e-182">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7e14e-183">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 Function Apps에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7e14e-184">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-185">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-185">Container</span></span>
* <span data-ttu-id="7e14e-186">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-186">Added `container start` command</span></span>
* <span data-ttu-id="7e14e-187">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7e14e-188">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7e14e-188">EventGrid</span></span>
* <span data-ttu-id="7e14e-189">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7e14e-190">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7e14e-191">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7e14e-192">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7e14e-193">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7e14e-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7e14e-194">HDInsight</span></span>
* <span data-ttu-id="7e14e-195">[주요 변경 내용] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7e14e-196">[주요 변경 내용] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7e14e-197">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7e14e-198">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7e14e-199">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7e14e-200">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-201">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-201">IoT</span></span>
* <span data-ttu-id="7e14e-202">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7e14e-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="7e14e-203">Kusto</span></span>
* <span data-ttu-id="7e14e-204">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-205">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-205">Monitor</span></span>
* <span data-ttu-id="7e14e-206">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-207">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-207">Profile</span></span>
* <span data-ttu-id="7e14e-208">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-209">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-209">Network</span></span>
* <span data-ttu-id="7e14e-210">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7e14e-211">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-212">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-212">Resource</span></span>
* <span data-ttu-id="7e14e-213">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7e14e-214">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7e14e-215">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="7e14e-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="7e14e-216">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-217">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-217">Storage</span></span>
* <span data-ttu-id="7e14e-218">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7e14e-219">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-220">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-220">VM</span></span>
* <span data-ttu-id="7e14e-221">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7e14e-222">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7e14e-223">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="7e14e-223">January 15, 2019</span></span>

<span data-ttu-id="7e14e-224">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7e14e-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-225">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-225">ACR</span></span>
* <span data-ttu-id="7e14e-226">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7e14e-227">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7e14e-228">[사용되지 않음] `--resource-group` 매개 변수가 다음 명령에서 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7e14e-229">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-229">ACS</span></span>
* <span data-ttu-id="7e14e-230">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-231">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-231">Appservice</span></span>
* <span data-ttu-id="7e14e-232">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7e14e-233">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7e14e-234">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7e14e-235">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7e14e-236">Botservice</span><span class="sxs-lookup"><span data-stu-id="7e14e-236">Botservice</span></span>
* <span data-ttu-id="7e14e-237">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7e14e-238">구성</span><span class="sxs-lookup"><span data-stu-id="7e14e-238">Configure</span></span>
* <span data-ttu-id="7e14e-239">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-240">CosmosDB</span></span>
* <span data-ttu-id="7e14e-241">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7e14e-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7e14e-242">HDInsight</span></span>
* <span data-ttu-id="7e14e-243">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-243">Added commands for managing applications</span></span>
* <span data-ttu-id="7e14e-244">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="7e14e-245">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7e14e-246">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7e14e-247">[주요 변경 내용] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-248">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-248">Network</span></span>
* <span data-ttu-id="7e14e-249">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7e14e-250">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7e14e-251">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7e14e-252">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-253">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-253">Role</span></span>
* <span data-ttu-id="7e14e-254">[사용되지 않음] `--password` 인수가 `create-for-rbac`에 대해 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7e14e-255">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7e14e-256">보안</span><span class="sxs-lookup"><span data-stu-id="7e14e-256">Security</span></span>
* <span data-ttu-id="7e14e-257">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-258">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-258">Storage</span></span>
* <span data-ttu-id="7e14e-259">[주요 변경 내용] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7e14e-260">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7e14e-261">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7e14e-262">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7e14e-263">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-264">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-264">VM</span></span>
* <span data-ttu-id="7e14e-265">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7e14e-266">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7e14e-267">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7e14e-268">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7e14e-269">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7e14e-270">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7e14e-271">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="7e14e-271">December 20, 2018</span></span>

<span data-ttu-id="7e14e-272">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7e14e-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7e14e-273">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-273">Appservice</span></span>
* <span data-ttu-id="7e14e-274">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7e14e-275">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7e14e-276">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7e14e-277">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="7e14e-277">IoTCentral</span></span>
* <span data-ttu-id="7e14e-278">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-279">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-279">Role</span></span>
* <span data-ttu-id="7e14e-280">[주요 변경 내용] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-281">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-281">SQL</span></span>
* <span data-ttu-id="7e14e-282">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-283">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-283">VM</span></span>
* <span data-ttu-id="7e14e-284">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7e14e-285">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="7e14e-285">December 18, 2018</span></span>

<span data-ttu-id="7e14e-286">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7e14e-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7e14e-287">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-287">ACR</span></span>
* <span data-ttu-id="7e14e-288">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7e14e-289">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="7e14e-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7e14e-290">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-291">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-291">ACS</span></span>
* <span data-ttu-id="7e14e-292">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7e14e-293">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="7e14e-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7e14e-294">[사용되지 않음] `az acs` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7e14e-295">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7e14e-296">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7e14e-297">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="7e14e-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-298">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-298">Appservice</span></span>
* <span data-ttu-id="7e14e-299">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7e14e-300">Botservice</span><span class="sxs-lookup"><span data-stu-id="7e14e-300">Botservice</span></span>
* <span data-ttu-id="7e14e-301">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7e14e-302">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="7e14e-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7e14e-303">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="7e14e-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7e14e-304">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="7e14e-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7e14e-305">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-306">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-306">Consumption</span></span>
* <span data-ttu-id="7e14e-307">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-308">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-308">CosmosDB</span></span>
* <span data-ttu-id="7e14e-309">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7e14e-310">지도</span><span class="sxs-lookup"><span data-stu-id="7e14e-310">Maps</span></span>
* <span data-ttu-id="7e14e-311">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-312">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-312">Network</span></span>
* <span data-ttu-id="7e14e-313">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7e14e-314">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="7e14e-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-315">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-315">Resource</span></span>
* <span data-ttu-id="7e14e-316">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7e14e-317">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-318">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-318">Storage</span></span>
*  <span data-ttu-id="7e14e-319">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-320">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-320">VM</span></span>
* <span data-ttu-id="7e14e-321">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7e14e-322">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="7e14e-322">December 4, 2018</span></span>

<span data-ttu-id="7e14e-323">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7e14e-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7e14e-324">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-324">Core</span></span>
* <span data-ttu-id="7e14e-325">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7e14e-326">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-327">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-327">Appservice</span></span>
* <span data-ttu-id="7e14e-328">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7e14e-329">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-330">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-330">Network</span></span>
* <span data-ttu-id="7e14e-331">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-332">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-332">Role</span></span>
* <span data-ttu-id="7e14e-333">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7e14e-334">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-334">VM</span></span>
* <span data-ttu-id="7e14e-335">[사용되지 않음]`vm extension [show|wait] --expand` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7e14e-336">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7e14e-337">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7e14e-338">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7e14e-339">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="7e14e-339">November 20, 2018</span></span>

<span data-ttu-id="7e14e-340">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7e14e-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7e14e-341">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-341">Core</span></span>
* <span data-ttu-id="7e14e-342">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-343">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-343">ACR</span></span>
* <span data-ttu-id="7e14e-344">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-344">Added context token to task step</span></span>
* <span data-ttu-id="7e14e-345">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7e14e-346">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-347">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-347">Appservice</span></span>
* <span data-ttu-id="7e14e-348">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7e14e-349">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-349">Updated the default `node_version`.</span></span> <span data-ttu-id="7e14e-350">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7e14e-351">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7e14e-352">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7e14e-353">IotCentral</span><span class="sxs-lookup"><span data-stu-id="7e14e-353">IotCentral</span></span>
* <span data-ttu-id="7e14e-354">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7e14e-355">KeyVault</span></span>
* <span data-ttu-id="7e14e-356">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-357">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-357">Network</span></span>
* <span data-ttu-id="7e14e-358">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7e14e-359">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="7e14e-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7e14e-360">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7e14e-361">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="7e14e-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7e14e-362">Rdbms</span></span>
* <span data-ttu-id="7e14e-363">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7e14e-364">Rbac</span><span class="sxs-lookup"><span data-stu-id="7e14e-364">Rbac</span></span>
* <span data-ttu-id="7e14e-365">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7e14e-366">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7e14e-367">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-367">Storage</span></span>
* <span data-ttu-id="7e14e-368">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7e14e-369">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7e14e-370">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7e14e-371">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-372">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-372">VM</span></span>
* <span data-ttu-id="7e14e-373">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7e14e-374">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7e14e-375">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7e14e-376">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7e14e-377">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7e14e-378">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7e14e-379">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7e14e-380">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="7e14e-380">November 6, 2018</span></span>

<span data-ttu-id="7e14e-381">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7e14e-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-382">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-382">Core</span></span>
* <span data-ttu-id="7e14e-383">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-384">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-384">ACR</span></span>
* <span data-ttu-id="7e14e-385">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7e14e-386">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-387">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-387">ACS</span></span>
* <span data-ttu-id="7e14e-388">[주요 변경 내용] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7e14e-389">Advisor</span><span class="sxs-lookup"><span data-stu-id="7e14e-389">Advisor</span></span>
* <span data-ttu-id="7e14e-390">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7e14e-391">AMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-391">AMS</span></span>
* <span data-ttu-id="7e14e-392">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="7e14e-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7e14e-393">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="7e14e-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7e14e-394">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7e14e-395">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7e14e-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7e14e-396">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7e14e-397">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7e14e-398">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7e14e-399">[주요 변경 내용] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7e14e-400">[주요 변경 내용] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7e14e-401">[주요 변경 내용] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7e14e-402">[주요 변경 내용] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7e14e-403">[주요 변경 내용] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7e14e-404">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="7e14e-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7e14e-405">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="7e14e-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7e14e-406">[주요 변경 내용] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7e14e-407">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7e14e-408">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-409">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-409">AppService</span></span>
* <span data-ttu-id="7e14e-410">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7e14e-411">구성</span><span class="sxs-lookup"><span data-stu-id="7e14e-411">Configure</span></span>
* <span data-ttu-id="7e14e-412">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-413">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-413">Container</span></span>
* <span data-ttu-id="7e14e-414">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7e14e-415">EventHub</span><span class="sxs-lookup"><span data-stu-id="7e14e-415">EventHub</span></span>
* <span data-ttu-id="7e14e-416">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-417">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-417">Interactive</span></span>
* <span data-ttu-id="7e14e-418">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-419">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-419">Monitor</span></span>
* <span data-ttu-id="7e14e-420">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-421">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-421">Network</span></span>
* <span data-ttu-id="7e14e-422">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7e14e-423">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7e14e-424">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7e14e-425">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-425">Profile</span></span>
* <span data-ttu-id="7e14e-426">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-427">RDBMS</span></span>
* <span data-ttu-id="7e14e-428">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-429">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-429">Resource</span></span>
* <span data-ttu-id="7e14e-430">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-431">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-431">Role</span></span>
* <span data-ttu-id="7e14e-432">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7e14e-433">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7e14e-434">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-435">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-435">Storage</span></span>
* <span data-ttu-id="7e14e-436">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-437">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-437">VM</span></span>
* <span data-ttu-id="7e14e-438">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7e14e-439">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7e14e-440">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7e14e-441">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7e14e-442">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="7e14e-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7e14e-443">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7e14e-444">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="7e14e-444">October 23, 2018</span></span>

<span data-ttu-id="7e14e-445">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7e14e-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-446">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-446">Core</span></span>
* <span data-ttu-id="7e14e-447">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7e14e-448">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-449">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-449">ACR</span></span>
* <span data-ttu-id="7e14e-450">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7e14e-451">CDN</span><span class="sxs-lookup"><span data-stu-id="7e14e-451">CDN</span></span>
* <span data-ttu-id="7e14e-452">[주요 변경 내용] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7e14e-453">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-454">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-454">Container</span></span>
* <span data-ttu-id="7e14e-455">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7e14e-456">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7e14e-457">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7e14e-458">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7e14e-459">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7e14e-460">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7e14e-461">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-462">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-462">CosmosDB</span></span>
* <span data-ttu-id="7e14e-463">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-464">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-464">Interactive</span></span>
* <span data-ttu-id="7e14e-465">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7e14e-466">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7e14e-466">IoT Central</span></span>
* <span data-ttu-id="7e14e-467">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7e14e-468">[주요 변경 내용] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-469">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-469">Monitor</span></span>
* <span data-ttu-id="7e14e-470">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7e14e-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7e14e-471">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7e14e-472">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7e14e-473">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7e14e-474">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7e14e-475">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7e14e-476">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7e14e-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7e14e-477">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7e14e-478">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7e14e-479">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-480">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-480">Network</span></span>
* <span data-ttu-id="7e14e-481">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7e14e-482">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7e14e-483">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7e14e-483">ServiceBus</span></span>
* <span data-ttu-id="7e14e-484">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-485">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-485">SQL</span></span>
* <span data-ttu-id="7e14e-486">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-487">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-487">Storage</span></span>
* <span data-ttu-id="7e14e-488">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7e14e-489">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-490">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-490">VM</span></span>
* <span data-ttu-id="7e14e-491">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7e14e-492">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7e14e-493">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7e14e-494">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="7e14e-494">October 16, 2018</span></span>

<span data-ttu-id="7e14e-495">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7e14e-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-496">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-496">VM</span></span>
* <span data-ttu-id="7e14e-497">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7e14e-498">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="7e14e-498">October 9, 2018</span></span>

<span data-ttu-id="7e14e-499">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7e14e-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-500">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-500">Core</span></span>
* <span data-ttu-id="7e14e-501">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-502">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-502">ACR</span></span>
* <span data-ttu-id="7e14e-503">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-504">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-504">ACS</span></span>
* <span data-ttu-id="7e14e-505">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="7e14e-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7e14e-506">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7e14e-507">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7e14e-508">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-509">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-509">Container</span></span>
* <span data-ttu-id="7e14e-510">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7e14e-511">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7e14e-512">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="7e14e-512">Event Hub</span></span>
* <span data-ttu-id="7e14e-513">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7e14e-514">[주요 변경 내용] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7e14e-515">확장</span><span class="sxs-lookup"><span data-stu-id="7e14e-515">Extensions</span></span>
* <span data-ttu-id="7e14e-516">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7e14e-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7e14e-517">HDInsight</span></span>
* <span data-ttu-id="7e14e-518">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-519">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-519">IoT</span></span>
* <span data-ttu-id="7e14e-520">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-521">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7e14e-521">KeyVault</span></span>
* <span data-ttu-id="7e14e-522">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-523">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-523">Network</span></span>
* <span data-ttu-id="7e14e-524">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7e14e-525">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="7e14e-525">See #6052</span></span>
* <span data-ttu-id="7e14e-526">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7e14e-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7e14e-527">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7e14e-528">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7e14e-529">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7e14e-530">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7e14e-531">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-532">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-532">Role</span></span>
* <span data-ttu-id="7e14e-533">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7e14e-534">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7e14e-535">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7e14e-536">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7e14e-537">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7e14e-537">Service Bus</span></span>
* <span data-ttu-id="7e14e-538">[주요 변경 내용] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-539">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-539">VM</span></span>
* <span data-ttu-id="7e14e-540">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7e14e-541">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7e14e-542">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7e14e-543">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7e14e-544">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7e14e-545">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7e14e-546">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="7e14e-546">September 21, 2018</span></span>

<span data-ttu-id="7e14e-547">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7e14e-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-548">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-548">ACR</span></span>
* <span data-ttu-id="7e14e-549">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-549">Added ACR Task commands</span></span>
* <span data-ttu-id="7e14e-550">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-550">Added quick run command</span></span>
* <span data-ttu-id="7e14e-551">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7e14e-552">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7e14e-553">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7e14e-554">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-555">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-555">ACS</span></span>
* <span data-ttu-id="7e14e-556">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7e14e-557">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-558">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-558">AppService</span></span>

* <span data-ttu-id="7e14e-559">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7e14e-560">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7e14e-561">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7e14e-562">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-563">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-563">Batch</span></span>
* <span data-ttu-id="7e14e-564">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7e14e-565">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7e14e-566">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7e14e-567">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7e14e-568">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7e14e-568">Batch AI</span></span> 
* <span data-ttu-id="7e14e-569">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7e14e-570">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7e14e-570">Cognitive Services</span></span>
* <span data-ttu-id="7e14e-571">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7e14e-572">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7e14e-573">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7e14e-574">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7e14e-575">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7e14e-576">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-577">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-577">Container</span></span>
* <span data-ttu-id="7e14e-578">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7e14e-579">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7e14e-580">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7e14e-581">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7e14e-582">Datalake</span><span class="sxs-lookup"><span data-stu-id="7e14e-582">Datalake</span></span>
* <span data-ttu-id="7e14e-583">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7e14e-584">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="7e14e-584">Interactive Shell</span></span>
* <span data-ttu-id="7e14e-585">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7e14e-586">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-587">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-587">IoT</span></span>
* <span data-ttu-id="7e14e-588">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7e14e-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7e14e-589">Key Vault</span></span>
* <span data-ttu-id="7e14e-590">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-591">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-591">Network</span></span>
* <span data-ttu-id="7e14e-592">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7e14e-593">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7e14e-594">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7e14e-595">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7e14e-596">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7e14e-597">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7e14e-598">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7e14e-599">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7e14e-600">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7e14e-601">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7e14e-602">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7e14e-603">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7e14e-604">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7e14e-605">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하는 논리가 수정됨. 사설 IP 주소가 제공되는 경우 정적 할당이 설정됨. 사설 IP 주소가 제공되지 않는 경우나 사설 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="7e14e-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7e14e-606">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7e14e-607">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7e14e-608">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7e14e-609">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-610">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-610">RDBMS</span></span>
* <span data-ttu-id="7e14e-611">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7e14e-612">예약</span><span class="sxs-lookup"><span data-stu-id="7e14e-612">Reservation</span></span>
* <span data-ttu-id="7e14e-613">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7e14e-614">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7e14e-615">앱 관리</span><span class="sxs-lookup"><span data-stu-id="7e14e-615">Manage App</span></span>
* <span data-ttu-id="7e14e-616">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7e14e-617">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-618">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-618">Role</span></span>
* <span data-ttu-id="7e14e-619">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7e14e-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="7e14e-620">SignalR</span></span>
* <span data-ttu-id="7e14e-621">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-622">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-622">Storage</span></span>
* <span data-ttu-id="7e14e-623">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7e14e-624">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-625">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-625">VM</span></span>
* <span data-ttu-id="7e14e-626">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="7e14e-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7e14e-627">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7e14e-628">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="7e14e-628">August 28, 2018</span></span>

<span data-ttu-id="7e14e-629">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7e14e-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-630">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-630">Core</span></span>

* <span data-ttu-id="7e14e-631">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7e14e-632">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-633">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-633">ACR</span></span>

* <span data-ttu-id="7e14e-634">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7e14e-635">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-636">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-636">ACS</span></span>

* <span data-ttu-id="7e14e-637">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7e14e-638">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-639">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-639">AppService</span></span>

* <span data-ttu-id="7e14e-640">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7e14e-641">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7e14e-642">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7e14e-643">Backup</span><span class="sxs-lookup"><span data-stu-id="7e14e-643">Backup</span></span>

* <span data-ttu-id="7e14e-644">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7e14e-645">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="7e14e-645">Bot Service</span></span>

* <span data-ttu-id="7e14e-646">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7e14e-647">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7e14e-647">Cognitive Services</span></span>

* <span data-ttu-id="7e14e-648">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-649">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-649">IoT</span></span>

* <span data-ttu-id="7e14e-650">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-651">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-651">Monitor</span></span>

* <span data-ttu-id="7e14e-652">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7e14e-653">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="7e14e-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-654">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-654">Network</span></span>

* <span data-ttu-id="7e14e-655">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-656">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-656">Resource</span></span>

* <span data-ttu-id="7e14e-657">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-658">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-658">Storage</span></span>

* <span data-ttu-id="7e14e-659">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-660">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-660">VM</span></span>

* <span data-ttu-id="7e14e-661">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7e14e-662">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7e14e-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7e14e-663">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="7e14e-663">Auguest 14, 2018</span></span>

<span data-ttu-id="7e14e-664">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7e14e-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-665">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-665">Core</span></span>

* <span data-ttu-id="7e14e-666">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7e14e-667">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="7e14e-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7e14e-668">원격 분석</span><span class="sxs-lookup"><span data-stu-id="7e14e-668">Telemetry</span></span>

* <span data-ttu-id="7e14e-669">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="7e14e-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-670">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-670">ACR</span></span>

* <span data-ttu-id="7e14e-671">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7e14e-672">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-673">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-673">ACS</span></span>

* <span data-ttu-id="7e14e-674">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7e14e-675">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7e14e-676">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7e14e-677">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7e14e-678">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7e14e-679">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-679">AppService</span></span>

* <span data-ttu-id="7e14e-680">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7e14e-681">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7e14e-682">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7e14e-682">BatchAI</span></span>

* <span data-ttu-id="7e14e-683">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7e14e-684">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-684">Container</span></span>

* <span data-ttu-id="7e14e-685">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7e14e-686">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-686">IoT</span></span>

* <span data-ttu-id="7e14e-687">[주요 변경 내용] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="7e14e-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7e14e-688">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7e14e-689">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7e14e-689">Iot Central</span></span>

* <span data-ttu-id="7e14e-690">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-691">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7e14e-691">KeyVault</span></span>


* <span data-ttu-id="7e14e-692">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7e14e-693">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7e14e-694">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7e14e-695">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7e14e-696">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7e14e-697">릴레이</span><span class="sxs-lookup"><span data-stu-id="7e14e-697">Relay</span></span>

* <span data-ttu-id="7e14e-698">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-699">Sql</span><span class="sxs-lookup"><span data-stu-id="7e14e-699">Sql</span></span>

* <span data-ttu-id="7e14e-700">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-701">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-701">Storage</span></span>

* <span data-ttu-id="7e14e-702">[주요 변경 내용] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7e14e-703">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7e14e-704">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7e14e-705">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7e14e-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7e14e-706">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-707">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-707">VM</span></span>

* <span data-ttu-id="7e14e-708">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7e14e-709">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="7e14e-709">July 31, 2018</span></span>

<span data-ttu-id="7e14e-710">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7e14e-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-711">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-711">ACR</span></span>

* <span data-ttu-id="7e14e-712">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7e14e-713">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-714">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-714">ACS</span></span>

* <span data-ttu-id="7e14e-715">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-716">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-716">Batch</span></span>

* <span data-ttu-id="7e14e-717">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-718">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-718">Container</span></span>

* <span data-ttu-id="7e14e-719">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-720">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-720">Network</span></span>

* <span data-ttu-id="7e14e-721">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7e14e-722">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-722">Resource</span></span>

* <span data-ttu-id="7e14e-723">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="7e14e-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7e14e-724">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-725">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-725">Role</span></span>

* <span data-ttu-id="7e14e-726">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7e14e-727">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7e14e-728">검색</span><span class="sxs-lookup"><span data-stu-id="7e14e-728">Search</span></span>

* <span data-ttu-id="7e14e-729">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7e14e-730">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7e14e-730">Service Bus</span></span>

* <span data-ttu-id="7e14e-731">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7e14e-732">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7e14e-733">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="7e14e-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7e14e-734">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="7e14e-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-735">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-735">Storage</span></span>

* <span data-ttu-id="7e14e-736">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7e14e-737">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="7e14e-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-738">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-738">VM</span></span>

* <span data-ttu-id="7e14e-739">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7e14e-740">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7e14e-741">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7e14e-742">[주요 변경 내용] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7e14e-743">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="7e14e-743">July 18, 2018</span></span>

<span data-ttu-id="7e14e-744">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7e14e-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-745">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-745">Core</span></span>

* <span data-ttu-id="7e14e-746">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7e14e-747">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7e14e-748">[주요 변경 내용] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-749">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-749">ACR</span></span>

* <span data-ttu-id="7e14e-750">[주요 변경 내용] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7e14e-751">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7e14e-752">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7e14e-753">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-754">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-754">ACS</span></span>

* <span data-ttu-id="7e14e-755">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-756">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-756">AppService</span></span>

* <span data-ttu-id="7e14e-757">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-758">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-758">Batch</span></span>

* <span data-ttu-id="7e14e-759">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7e14e-760">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7e14e-761">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7e14e-761">Batch AI</span></span>

* <span data-ttu-id="7e14e-762">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-763">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-763">Container</span></span>

* <span data-ttu-id="7e14e-764">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7e14e-765">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-766">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-766">Network</span></span>

* <span data-ttu-id="7e14e-767">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7e14e-768">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-768">Added `network nic wait`</span></span>
* <span data-ttu-id="7e14e-769">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7e14e-770">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7e14e-771">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-771">Resource</span></span>

* <span data-ttu-id="7e14e-772">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7e14e-773">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7e14e-774">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="7e14e-775">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-776">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-776">SQL</span></span>

* <span data-ttu-id="7e14e-777">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7e14e-778">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7e14e-779">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="7e14e-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-780">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-780">Storage</span></span>

* <span data-ttu-id="7e14e-781">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-782">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-782">VM</span></span>

* <span data-ttu-id="7e14e-783">[주요 변경 내용] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7e14e-784">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7e14e-785">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7e14e-786">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="7e14e-786">July 3, 2018</span></span>

<span data-ttu-id="7e14e-787">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7e14e-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7e14e-788">AKS</span><span class="sxs-lookup"><span data-stu-id="7e14e-788">AKS</span></span>

* <span data-ttu-id="7e14e-789">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7e14e-790">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="7e14e-790">July 3, 2018</span></span>

<span data-ttu-id="7e14e-791">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7e14e-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-792">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-792">Core</span></span>

* <span data-ttu-id="7e14e-793">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-794">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-794">ACR</span></span>

* <span data-ttu-id="7e14e-795">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-795">Added polling build status</span></span>
* <span data-ttu-id="7e14e-796">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7e14e-797">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-798">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-798">ACS</span></span>

* <span data-ttu-id="7e14e-799">[주요 변경 내용]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7e14e-800">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7e14e-801">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="7e14e-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7e14e-802">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="7e14e-803">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="7e14e-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7e14e-804">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="7e14e-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7e14e-805">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-806">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-806">AppService</span></span>

* <span data-ttu-id="7e14e-807">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7e14e-808">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7e14e-809">Backup</span><span class="sxs-lookup"><span data-stu-id="7e14e-809">Backup</span></span>

* <span data-ttu-id="7e14e-810">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7e14e-811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7e14e-811">BatchAI</span></span>

* <span data-ttu-id="7e14e-812">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7e14e-813">클라우드</span><span class="sxs-lookup"><span data-stu-id="7e14e-813">Cloud</span></span>

* <span data-ttu-id="7e14e-814">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-815">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-815">Container</span></span>

* <span data-ttu-id="7e14e-816">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7e14e-817">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7e14e-818">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-819">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-819">Extension</span></span>

* <span data-ttu-id="7e14e-820">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-821">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-821">Network</span></span>

* <span data-ttu-id="7e14e-822">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7e14e-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7e14e-823">Rdbms</span></span>

* <span data-ttu-id="7e14e-824">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-825">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-825">Resource</span></span>

* <span data-ttu-id="7e14e-826">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-827">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-827">VM</span></span>

* <span data-ttu-id="7e14e-828">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7e14e-829">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="7e14e-829">June 25, 2018</span></span>

<span data-ttu-id="7e14e-830">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7e14e-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7e14e-831">CLI</span><span class="sxs-lookup"><span data-stu-id="7e14e-831">CLI</span></span>

* <span data-ttu-id="7e14e-832">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7e14e-833">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="7e14e-833">June 19, 2018</span></span>

<span data-ttu-id="7e14e-834">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7e14e-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-835">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-835">Core</span></span>

* <span data-ttu-id="7e14e-836">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-837">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-837">ACR</span></span>

* <span data-ttu-id="7e14e-838">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7e14e-839">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-840">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-840">ACS</span></span>

* <span data-ttu-id="7e14e-841">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="7e14e-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7e14e-842">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-842">Added `--update` support</span></span>
* <span data-ttu-id="7e14e-843">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7e14e-844">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="7e14e-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7e14e-845">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7e14e-846">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7e14e-847">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7e14e-848">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-849">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-849">AppService</span></span>

* <span data-ttu-id="7e14e-850">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7e14e-851">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-852">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-852">Batch</span></span>

* <span data-ttu-id="7e14e-853">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7e14e-854">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7e14e-854">Batch AI</span></span>

* <span data-ttu-id="7e14e-855">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7e14e-855">Added support for workspaces.</span></span> <span data-ttu-id="7e14e-856">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7e14e-857">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7e14e-857">Added support for experiments.</span></span> <span data-ttu-id="7e14e-858">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7e14e-859">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7e14e-860">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="7e14e-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7e14e-861">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7e14e-862">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7e14e-863">[주요 변경 내용] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="7e14e-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7e14e-864">[주요 변경 내용] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="7e14e-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7e14e-865">[주요 변경 내용] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="7e14e-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7e14e-866">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="7e14e-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7e14e-867">[주요 변경 내용] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="7e14e-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7e14e-868">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="7e14e-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7e14e-869">[주요 변경 내용] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="7e14e-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7e14e-870">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7e14e-871">[주요 변경 내용] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7e14e-872">[주요 변경 내용] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="7e14e-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7e14e-873">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7e14e-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7e14e-874">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7e14e-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7e14e-875">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7e14e-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7e14e-876">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7e14e-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7e14e-877">지도</span><span class="sxs-lookup"><span data-stu-id="7e14e-877">Maps</span></span>

* <span data-ttu-id="7e14e-878">[주요 변경 내용] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-879">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-879">Network</span></span>

* <span data-ttu-id="7e14e-880">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7e14e-881">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7e14e-882">#6502</span><span class="sxs-lookup"><span data-stu-id="7e14e-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7e14e-883">예약</span><span class="sxs-lookup"><span data-stu-id="7e14e-883">Reservations</span></span>

* <span data-ttu-id="7e14e-884">[주요 변경 내용] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7e14e-885">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7e14e-886">[주요 변경 내용] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7e14e-887">[주요 변경 내용] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7e14e-888">[주요 변경 내용] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7e14e-889">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-890">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-890">Role</span></span>

* <span data-ttu-id="7e14e-891">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="7e14e-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-892">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-892">SQL</span></span>

* <span data-ttu-id="7e14e-893">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-894">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-894">Storage</span></span>

* <span data-ttu-id="7e14e-895">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="7e14e-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-896">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-896">VM</span></span>

* <span data-ttu-id="7e14e-897">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7e14e-898">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7e14e-899">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7e14e-900">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="7e14e-900">June 13, 2018</span></span>

<span data-ttu-id="7e14e-901">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7e14e-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-902">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-902">Core</span></span>

* <span data-ttu-id="7e14e-903">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="7e14e-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7e14e-904">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="7e14e-904">June 13, 2018</span></span>

<span data-ttu-id="7e14e-905">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7e14e-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7e14e-906">AKS</span><span class="sxs-lookup"><span data-stu-id="7e14e-906">AKS</span></span>

* <span data-ttu-id="7e14e-907">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7e14e-908">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="7e14e-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7e14e-909">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7e14e-910">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7e14e-911">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-912">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-912">AppService</span></span>

* <span data-ttu-id="7e14e-913">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7e14e-914">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="7e14e-914">June 5, 2018</span></span>

<span data-ttu-id="7e14e-915">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7e14e-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-916">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-916">Interactive</span></span>

* <span data-ttu-id="7e14e-917">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="7e14e-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7e14e-918">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="7e14e-918">June 5, 2018</span></span>

<span data-ttu-id="7e14e-919">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7e14e-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-920">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-920">Core</span></span>

* <span data-ttu-id="7e14e-921">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7e14e-922">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-923">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-923">ACR</span></span>

* <span data-ttu-id="7e14e-924">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7e14e-925">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7e14e-926">AKS</span><span class="sxs-lookup"><span data-stu-id="7e14e-926">AKS</span></span>

* <span data-ttu-id="7e14e-927">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-928">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-928">Batch</span></span>

* <span data-ttu-id="7e14e-929">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7e14e-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-930">IOT</span><span class="sxs-lookup"><span data-stu-id="7e14e-930">IOT</span></span>

* <span data-ttu-id="7e14e-931">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-932">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-932">Network</span></span>

* <span data-ttu-id="7e14e-933">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="7e14e-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7e14e-934">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="7e14e-934">Policy Insights</span></span>

* <span data-ttu-id="7e14e-935">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7e14e-936">ARM</span><span class="sxs-lookup"><span data-stu-id="7e14e-936">ARM</span></span>

* <span data-ttu-id="7e14e-937">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-938">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-938">SQL</span></span>

* <span data-ttu-id="7e14e-939">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="7e14e-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7e14e-940">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7e14e-941">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-941">Storage</span></span>

* <span data-ttu-id="7e14e-942">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="7e14e-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-943">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-943">VM</span></span>

* <span data-ttu-id="7e14e-944">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7e14e-945">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7e14e-946">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7e14e-947">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="7e14e-947">May 22, 2018</span></span>

<span data-ttu-id="7e14e-948">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7e14e-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-949">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-949">Core</span></span>

* <span data-ttu-id="7e14e-950">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-951">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-951">ACS</span></span>

* <span data-ttu-id="7e14e-952">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7e14e-953">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-954">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-954">AppService</span></span>

* <span data-ttu-id="7e14e-955">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-955">Improved generic update commands</span></span>
* <span data-ttu-id="7e14e-956">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-957">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-957">Container</span></span>

* <span data-ttu-id="7e14e-958">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7e14e-959">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-960">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-960">Extension</span></span>

* <span data-ttu-id="7e14e-961">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-962">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-962">Interactive</span></span>

* <span data-ttu-id="7e14e-963">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7e14e-964">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="7e14e-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7e14e-965">KeyVault</span></span>

* <span data-ttu-id="7e14e-966">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="7e14e-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-967">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-967">Network</span></span>

* <span data-ttu-id="7e14e-968">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="7e14e-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7e14e-969">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-970">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-970">SQL</span></span>

* <span data-ttu-id="7e14e-971">[주요 변경 내용] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="7e14e-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7e14e-972">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="7e14e-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7e14e-973">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7e14e-974">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7e14e-975">[주요 변경 내용] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7e14e-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7e14e-977">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7e14e-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-978">`edition`.</span></span> <span data-ttu-id="7e14e-979">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7e14e-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-980">`elasticPoolName`.</span></span> <span data-ttu-id="7e14e-981">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7e14e-982">[주요 변경 내용] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7e14e-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-983">`edition`.</span></span> <span data-ttu-id="7e14e-984">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="7e14e-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7e14e-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-985">`dtu`.</span></span> <span data-ttu-id="7e14e-986">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="7e14e-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7e14e-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-987">`databaseDtuMin`.</span></span> <span data-ttu-id="7e14e-988">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="7e14e-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7e14e-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7e14e-989">`databaseDtuMax`.</span></span> <span data-ttu-id="7e14e-990">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="7e14e-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7e14e-991">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7e14e-992">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-993">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-993">Storage</span></span>

* <span data-ttu-id="7e14e-994">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7e14e-995">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-996">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-996">VM</span></span>

* <span data-ttu-id="7e14e-997">[주요 변경 내용] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="7e14e-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7e14e-998">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7e14e-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7e14e-999">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="7e14e-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7e14e-1000">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="7e14e-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7e14e-1001">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7e14e-1002">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1002">May 7, 2018</span></span>

<span data-ttu-id="7e14e-1003">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7e14e-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1004">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1004">Core</span></span>

* <span data-ttu-id="7e14e-1005">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7e14e-1006">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7e14e-1007">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7e14e-1008">#5591</span><span class="sxs-lookup"><span data-stu-id="7e14e-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7e14e-1009">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7e14e-1010">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7e14e-1011">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7e14e-1012">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7e14e-1013">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1014">ACR</span></span>

* <span data-ttu-id="7e14e-1015">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="7e14e-1016">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="7e14e-1017">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7e14e-1018">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7e14e-1019">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="7e14e-1020">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1021">ACS</span></span>

* <span data-ttu-id="7e14e-1022">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7e14e-1023">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7e14e-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1024">AMS</span></span>

* <span data-ttu-id="7e14e-1025">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="7e14e-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1026">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1026">Appservice</span></span>

* <span data-ttu-id="7e14e-1027">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7e14e-1028">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7e14e-1029">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7e14e-1030">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7e14e-1031">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7e14e-1031">Batch AI</span></span>

* <span data-ttu-id="7e14e-1032">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7e14e-1033">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7e14e-1033">Cognitive Services</span></span>

* <span data-ttu-id="7e14e-1034">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-1035">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-1035">Consumption</span></span>

* <span data-ttu-id="7e14e-1036">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1037">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1037">Container</span></span>

* <span data-ttu-id="7e14e-1038">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7e14e-1039">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7e14e-1039">Cosmos DB</span></span>

* <span data-ttu-id="7e14e-1040">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7e14e-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7e14e-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1041">DMS</span></span>

* <span data-ttu-id="7e14e-1042">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1043">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1043">Extension</span></span>

* <span data-ttu-id="7e14e-1044">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1045">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1045">Interactive</span></span>

* <span data-ttu-id="7e14e-1046">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7e14e-1047">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="7e14e-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7e14e-1048">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7e14e-1049">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7e14e-1050">랩</span><span class="sxs-lookup"><span data-stu-id="7e14e-1050">Lab</span></span>

* <span data-ttu-id="7e14e-1051">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1052">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1052">Network</span></span>

* <span data-ttu-id="7e14e-1053">[주요 변경 내용] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7e14e-1054">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1054">Profile</span></span>

* <span data-ttu-id="7e14e-1055">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7e14e-1056">[주요 변경 내용] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7e14e-1057">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7e14e-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="7e14e-1058">Redis</span></span>

* <span data-ttu-id="7e14e-1059">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7e14e-1060">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7e14e-1061">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7e14e-1062">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7e14e-1063">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1064">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1064">Role</span></span>

* <span data-ttu-id="7e14e-1065">[주요 변경 내용] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1066">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1066">Storage</span></span>

* <span data-ttu-id="7e14e-1067">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7e14e-1068">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="7e14e-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7e14e-1069">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="7e14e-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7e14e-1070">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7e14e-1071">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1072">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1072">VM</span></span>

* <span data-ttu-id="7e14e-1073">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7e14e-1074">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7e14e-1075">[주요 변경 내용] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="7e14e-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7e14e-1076">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7e14e-1077">[주요 변경 내용] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7e14e-1078">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1078">Added write accelerator support</span></span>
* <span data-ttu-id="7e14e-1079">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7e14e-1080">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7e14e-1081">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7e14e-1082">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1082">April 10, 2018</span></span>

<span data-ttu-id="7e14e-1083">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7e14e-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1084">ACR</span></span>

* <span data-ttu-id="7e14e-1085">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="7e14e-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1086">ACS</span></span>

* <span data-ttu-id="7e14e-1087">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1088">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1088">Appservice</span></span>

* [주요 변경 내용]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7e14e-1090">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7e14e-1091">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7e14e-1091">BatchAI</span></span>

* <span data-ttu-id="7e14e-1092">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7e14e-1093">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="7e14e-1093">Job level mounting</span></span>
  - <span data-ttu-id="7e14e-1094">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="7e14e-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="7e14e-1095">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1095">Performance counters settings</span></span>
  - <span data-ttu-id="7e14e-1096">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="7e14e-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7e14e-1097">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7e14e-1098">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="7e14e-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="7e14e-1099">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7e14e-1100">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1100">Support for custom images</span></span>
  - <span data-ttu-id="7e14e-1101">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7e14e-1102">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7e14e-1103">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7e14e-1104">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1104">National clouds are supported</span></span>
* <span data-ttu-id="7e14e-1105">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7e14e-1106">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7e14e-1107">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7e14e-1108">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7e14e-1109">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7e14e-1110">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7e14e-1111">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7e14e-1112">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7e14e-1113">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7e14e-1114">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7e14e-1115">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7e14e-1116">[주요 변경 내용] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7e14e-1117">[주요 변경 내용] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7e14e-1118">결제</span><span class="sxs-lookup"><span data-stu-id="7e14e-1118">Billing</span></span>

* <span data-ttu-id="7e14e-1119">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-1120">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-1120">Consumption</span></span>

* <span data-ttu-id="7e14e-1121">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="7e14e-1122">[주요 변경 내용] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7e14e-1123">[주요 변경 내용] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7e14e-1124">[주요 변경 내용] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7e14e-1125">[주요 변경 내용] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7e14e-1126">[주요 변경 내용] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1127">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1127">Container</span></span>

* <span data-ttu-id="7e14e-1128">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7e14e-1129">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="7e14e-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1130">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1130">Extension</span></span>

* <span data-ttu-id="7e14e-1131">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1132">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1132">Interactive</span></span>

* <span data-ttu-id="7e14e-1133">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7e14e-1134">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7e14e-1135">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1136">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1136">Network</span></span>

* <span data-ttu-id="7e14e-1137">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7e14e-1138">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7e14e-1139">#4910</span><span class="sxs-lookup"><span data-stu-id="7e14e-1139">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7e14e-1140">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7e14e-1141">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7e14e-1142">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7e14e-1143">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7e14e-1144">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1145">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1145">Profile</span></span>

* <span data-ttu-id="7e14e-1146">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7e14e-1147">[주요 변경 내용] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-1148">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1148">RDBMS</span></span>

* <span data-ttu-id="7e14e-1149">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1149">Added `georestore` command</span></span>
* <span data-ttu-id="7e14e-1150">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1151">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1151">Resource</span></span>

* <span data-ttu-id="7e14e-1152">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7e14e-1153">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1154">SQL</span></span>

* <span data-ttu-id="7e14e-1155">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1156">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1156">Storage</span></span>

* <span data-ttu-id="7e14e-1157">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1158">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1158">VM</span></span>

* <span data-ttu-id="7e14e-1159">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7e14e-1160">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7e14e-1162">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7e14e-1163">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7e14e-1164">#5718</span><span class="sxs-lookup"><span data-stu-id="7e14e-1164">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7e14e-1165">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7e14e-1166">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1166">March 27, 2018</span></span>

<span data-ttu-id="7e14e-1167">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7e14e-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1168">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1168">Core</span></span>

* <span data-ttu-id="7e14e-1169">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="7e14e-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1170">ACS</span></span>

* <span data-ttu-id="7e14e-1171">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1172">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1172">Appservice</span></span>

* <span data-ttu-id="7e14e-1173">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7e14e-1174">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7e14e-1175">Backup</span><span class="sxs-lookup"><span data-stu-id="7e14e-1175">Backup</span></span>

* <span data-ttu-id="7e14e-1176">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7e14e-1177">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7e14e-1178">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="7e14e-1179">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1180">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1180">Container</span></span>

* <span data-ttu-id="7e14e-1181">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1181">Added `container exec` command.</span></span> <span data-ttu-id="7e14e-1182">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7e14e-1183">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1184">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1184">Extension</span></span>

* <span data-ttu-id="7e14e-1185">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7e14e-1186">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7e14e-1187">[주요 변경 내용] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1188">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1188">Interactive</span></span>

* <span data-ttu-id="7e14e-1189">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="7e14e-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7e14e-1190">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7e14e-1191">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7e14e-1192">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7e14e-1193">랩</span><span class="sxs-lookup"><span data-stu-id="7e14e-1193">Lab</span></span>

* <span data-ttu-id="7e14e-1194">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1195">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1195">Monitor</span></span>

* <span data-ttu-id="7e14e-1196">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7e14e-1197">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7e14e-1198">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1199">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1199">Network</span></span>

* <span data-ttu-id="7e14e-1200">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1201">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1201">Profile</span></span>

* <span data-ttu-id="7e14e-1202">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-1203">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1203">RDBMS</span></span>

* <span data-ttu-id="7e14e-1204">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1205">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1205">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7e14e-1207">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1207">Role</span></span>

* <span data-ttu-id="7e14e-1208">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7e14e-1209">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7e14e-1210">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7e14e-1211">[주요 변경 내용] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7e14e-1212">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1213">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1213">Storage</span></span>

* <span data-ttu-id="7e14e-1214">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7e14e-1215">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="7e14e-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1216">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1216">VM</span></span>

* <span data-ttu-id="7e14e-1217">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7e14e-1218">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7e14e-1219">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7e14e-1220">[주요 변경 내용] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7e14e-1221">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1221">March 13, 2018</span></span>

<span data-ttu-id="7e14e-1222">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7e14e-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1223">ACR</span></span>

* <span data-ttu-id="7e14e-1224">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7e14e-1225">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7e14e-1226">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1227">ACS</span></span>

* <span data-ttu-id="7e14e-1228">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7e14e-1229">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7e14e-1230">Advisor</span><span class="sxs-lookup"><span data-stu-id="7e14e-1230">Advisor</span></span>

* <span data-ttu-id="7e14e-1231">[주요 변경 내용] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7e14e-1232">[주요 변경 내용] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7e14e-1233">[주요 변경 내용] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7e14e-1234">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7e14e-1235">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1236">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1236">Appservice</span></span>

* <span data-ttu-id="7e14e-1237">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7e14e-1238">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7e14e-1239">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7e14e-1239">Eventhubs</span></span>

* <span data-ttu-id="7e14e-1240">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1241">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1241">Extension</span></span>

* <span data-ttu-id="7e14e-1242">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1243">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1243">Interactive</span></span>

* <span data-ttu-id="7e14e-1244">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="7e14e-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7e14e-1245">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="7e14e-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7e14e-1246">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7e14e-1247">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1248">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1248">Monitor</span></span>

* <span data-ttu-id="7e14e-1249">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7e14e-1250">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7e14e-1251">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7e14e-1252">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1253">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1253">Network</span></span>

* <span data-ttu-id="7e14e-1254">[주요 변경 내용] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7e14e-1255">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="7e14e-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7e14e-1256">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7e14e-1257">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1258">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1258">Profile</span></span>

* <span data-ttu-id="7e14e-1259">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7e14e-1260">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-1261">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1261">RDBMS</span></span>

* <span data-ttu-id="7e14e-1262">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7e14e-1263">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7e14e-1263">Service Bus</span></span>

* <span data-ttu-id="7e14e-1264">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1265">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1265">Storage</span></span>

* <span data-ttu-id="7e14e-1266">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7e14e-1267">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1268">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1268">VM</span></span>

* <span data-ttu-id="7e14e-1269">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7e14e-1270">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7e14e-1271">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7e14e-1272">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7e14e-1273">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1273">February 27, 2018</span></span>

<span data-ttu-id="7e14e-1274">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7e14e-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1275">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1275">Core</span></span>

* <span data-ttu-id="7e14e-1276">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="7e14e-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7e14e-1277">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7e14e-1278">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1279">ACS</span></span>

* <span data-ttu-id="7e14e-1280">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7e14e-1281">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7e14e-1282">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7e14e-1283">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1284">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1284">Appservice</span></span>

* <span data-ttu-id="7e14e-1285">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7e14e-1286">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7e14e-1287">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7e14e-1287">Cognitive Services</span></span>

* <span data-ttu-id="7e14e-1288">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-1289">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-1289">Consumption</span></span>

* <span data-ttu-id="7e14e-1290">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7e14e-1291">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1292">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1292">Container</span></span>

* <span data-ttu-id="7e14e-1293">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1294">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1294">Network</span></span>

* <span data-ttu-id="7e14e-1295">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1296">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1296">Resource</span></span>

* <span data-ttu-id="7e14e-1297">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1298">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1298">Role</span></span>

* <span data-ttu-id="7e14e-1299">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1300">SQL</span></span>

* <span data-ttu-id="7e14e-1301">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1302">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1302">Storage</span></span>

* <span data-ttu-id="7e14e-1303">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1304">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1304">VM</span></span>

* <span data-ttu-id="7e14e-1305">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7e14e-1306">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1306">February 13, 2018</span></span>

<span data-ttu-id="7e14e-1307">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7e14e-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1308">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1308">Core</span></span>

* <span data-ttu-id="7e14e-1309">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1310">ACS</span></span>

* <span data-ttu-id="7e14e-1311">[주요 변경 내용] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7e14e-1312">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7e14e-1313">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7e14e-1314">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="7e14e-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7e14e-1315">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7e14e-1316">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7e14e-1317">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7e14e-1318">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1319">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1319">Appservice</span></span>

* <span data-ttu-id="7e14e-1320">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7e14e-1321">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7e14e-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="7e14e-1322">CDN</span></span>

* <span data-ttu-id="7e14e-1323">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1324">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1324">Container</span></span>

* <span data-ttu-id="7e14e-1325">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7e14e-1326">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-1327">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-1327">CosmosDB</span></span>

* <span data-ttu-id="7e14e-1328">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1329">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1329">Extension</span></span>

* <span data-ttu-id="7e14e-1330">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7e14e-1331">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7e14e-1332">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="7e14e-1332">Feedback</span></span>

* <span data-ttu-id="7e14e-1333">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1334">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1334">Interactive</span></span>

* <span data-ttu-id="7e14e-1335">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7e14e-1336">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-1337">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-1337">IoT</span></span>

* <span data-ttu-id="7e14e-1338">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7e14e-1339">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7e14e-1340">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7e14e-1341">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1342">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1342">Monitor</span></span>

* <span data-ttu-id="7e14e-1343">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1344">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1344">Network</span></span>

* <span data-ttu-id="7e14e-1345">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7e14e-1346">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1346">Profile</span></span>

* <span data-ttu-id="7e14e-1347">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1348">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1348">Resource</span></span>

* <span data-ttu-id="7e14e-1349">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1350">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1350">Role</span></span>

* <span data-ttu-id="7e14e-1351">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1352">SQL</span></span>

* <span data-ttu-id="7e14e-1353">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7e14e-1354">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="7e14e-1355">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1356">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1356">Storage</span></span>

* <span data-ttu-id="7e14e-1357">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1358">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1358">VM</span></span>

* <span data-ttu-id="7e14e-1359">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7e14e-1360">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7e14e-1361">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7e14e-1362">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1362">January 31, 2018</span></span>

<span data-ttu-id="7e14e-1363">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7e14e-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1364">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1364">Core</span></span>

* <span data-ttu-id="7e14e-1365">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7e14e-1366">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7e14e-1367">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7e14e-1368">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="7e14e-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="7e14e-1369">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1370">ACS</span></span>

* <span data-ttu-id="7e14e-1371">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7e14e-1372">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="7e14e-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1373">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1373">Appservice</span></span>

* <span data-ttu-id="7e14e-1374">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7e14e-1375">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7e14e-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="7e14e-1376">CDN</span></span>

* <span data-ttu-id="7e14e-1377">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-1378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-1378">CosmosDB</span></span>

* <span data-ttu-id="7e14e-1379">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1380">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1380">Interactive</span></span>

* <span data-ttu-id="7e14e-1381">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1382">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1382">Network</span></span>

* <span data-ttu-id="7e14e-1383">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7e14e-1384">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7e14e-1385">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7e14e-1386">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7e14e-1387">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7e14e-1388">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="7e14e-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7e14e-1389">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7e14e-1390">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7e14e-1391">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7e14e-1392">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1393">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1393">Profile</span></span>

* <span data-ttu-id="7e14e-1394">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1395">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1395">Resource</span></span>

* <span data-ttu-id="7e14e-1396">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1397">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1397">Storage</span></span>

* <span data-ttu-id="7e14e-1398">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7e14e-1399">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7e14e-1400">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7e14e-1401">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7e14e-1402">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1403">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1403">VM</span></span>

* <span data-ttu-id="7e14e-1404">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7e14e-1405">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7e14e-1406">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7e14e-1407">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7e14e-1408">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1408">January 17, 2018</span></span>

<span data-ttu-id="7e14e-1409">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7e14e-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1410">ACR</span></span>

* <span data-ttu-id="7e14e-1411">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7e14e-1412">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1413">ACS</span></span>

* <span data-ttu-id="7e14e-1414">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7e14e-1415">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1416">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1416">Appservice</span></span>

* <span data-ttu-id="7e14e-1417">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7e14e-1418">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7e14e-1419">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7e14e-1420">Backup</span><span class="sxs-lookup"><span data-stu-id="7e14e-1420">Backup</span></span>

* <span data-ttu-id="7e14e-1421">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7e14e-1422">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7e14e-1423">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7e14e-1424">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7e14e-1425">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-1426">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-1426">Batch</span></span>

* <span data-ttu-id="7e14e-1427">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7e14e-1428">클라우드</span><span class="sxs-lookup"><span data-stu-id="7e14e-1428">Cloud</span></span>

* <span data-ttu-id="7e14e-1429">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-1430">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-1430">Consumption</span></span>

* <span data-ttu-id="7e14e-1431">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7e14e-1432">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7e14e-1432">Event Grid</span></span>

* <span data-ttu-id="7e14e-1433">[주요 변경 내용] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7e14e-1434">[주요 변경 내용] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7e14e-1435">[주요 변경 내용] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7e14e-1436">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7e14e-1437">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7e14e-1438">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7e14e-1439">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7e14e-1440">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1441">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1441">Interactive</span></span>

* <span data-ttu-id="7e14e-1442">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7e14e-1443">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="7e14e-1444">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-1445">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-1445">IoT</span></span>

* <span data-ttu-id="7e14e-1446">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="7e14e-1447">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7e14e-1448">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1449">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1449">Monitor</span></span>

* <span data-ttu-id="7e14e-1450">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7e14e-1451">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="7e14e-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7e14e-1452">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1453">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1453">Network</span></span>

* <span data-ttu-id="7e14e-1454">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7e14e-1455">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1456">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1456">Profile</span></span>

* <span data-ttu-id="7e14e-1457">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1458">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1458">Role</span></span>

* <span data-ttu-id="7e14e-1459">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7e14e-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7e14e-1460">Service Fabric</span></span>

* <span data-ttu-id="7e14e-1461">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7e14e-1462">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1463">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1463">VM</span></span>

* <span data-ttu-id="7e14e-1464">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7e14e-1465">[주요 변경 내용] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7e14e-1466">[주요 변경 내용] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7e14e-1467">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7e14e-1468">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7e14e-1469">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7e14e-1470">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7e14e-1471">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7e14e-1472">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1472">December 19, 2017</span></span>

<span data-ttu-id="7e14e-1473">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7e14e-1473">Version 2.0.23</span></span>

* <span data-ttu-id="7e14e-1474">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1475">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1475">Container</span></span>

* <span data-ttu-id="7e14e-1476">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1477">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1477">Network</span></span>

* <span data-ttu-id="7e14e-1478">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7e14e-1479">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1480">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1480">Storage</span></span>

* <span data-ttu-id="7e14e-1481">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1482">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1482">VM</span></span>

* <span data-ttu-id="7e14e-1483">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7e14e-1484">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1484">December 5, 2017</span></span>

<span data-ttu-id="7e14e-1485">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7e14e-1485">Version 2.0.22</span></span>

* <span data-ttu-id="7e14e-1486">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1486">Removed `az component` commands.</span></span> <span data-ttu-id="7e14e-1487">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1488">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1488">Core</span></span>
* <span data-ttu-id="7e14e-1489">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7e14e-1490">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1491">ACS</span></span>

* <span data-ttu-id="7e14e-1492">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7e14e-1493">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7e14e-1494">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7e14e-1495">Advisor</span><span class="sxs-lookup"><span data-stu-id="7e14e-1495">Advisor</span></span>

* <span data-ttu-id="7e14e-1496">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1497">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1497">Appservice</span></span>

* <span data-ttu-id="7e14e-1498">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7e14e-1499">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7e14e-1500">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7e14e-1501">Consumption</span><span class="sxs-lookup"><span data-stu-id="7e14e-1501">Consumption</span></span>

* <span data-ttu-id="7e14e-1502">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1503">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1503">Container</span></span>

* <span data-ttu-id="7e14e-1504">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1505">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1505">Monitor</span></span>

* <span data-ttu-id="7e14e-1506">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1507">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1507">Resource</span></span>

* <span data-ttu-id="7e14e-1508">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1509">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1509">Role</span></span>

* <span data-ttu-id="7e14e-1510">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7e14e-1511">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7e14e-1512">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1513">SQL</span></span>

* <span data-ttu-id="7e14e-1514">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7e14e-1515">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1516">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1516">VM</span></span>

* <span data-ttu-id="7e14e-1517">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7e14e-1518">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1518">November 14, 2017</span></span>

<span data-ttu-id="7e14e-1519">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7e14e-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1520">ACR</span></span>

* <span data-ttu-id="7e14e-1521">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7e14e-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1522">ACS</span></span>

* <span data-ttu-id="7e14e-1523">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7e14e-1524">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="7e14e-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7e14e-1525">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7e14e-1526">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7e14e-1527">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1528">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1528">Appservice</span></span>

* <span data-ttu-id="7e14e-1529">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7e14e-1530">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7e14e-1531">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7e14e-1532">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7e14e-1533">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7e14e-1534">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-1535">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-1535">Batch</span></span>

* <span data-ttu-id="7e14e-1536">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7e14e-1537">Batchai</span><span class="sxs-lookup"><span data-stu-id="7e14e-1537">Batchai</span></span>

* <span data-ttu-id="7e14e-1538">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7e14e-1539">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7e14e-1540">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7e14e-1541">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7e14e-1542">클라우드</span><span class="sxs-lookup"><span data-stu-id="7e14e-1542">Cloud</span></span>

* <span data-ttu-id="7e14e-1543">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1544">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1544">Container</span></span>

* <span data-ttu-id="7e14e-1545">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="7e14e-1546">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1546">Added container group restart policy</span></span>
* <span data-ttu-id="7e14e-1547">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7e14e-1548">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="7e14e-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7e14e-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7e14e-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="7e14e-1550">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7e14e-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7e14e-1551">Data Lake Store</span></span>

* <span data-ttu-id="7e14e-1552">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1553">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1553">Extension</span></span>

* <span data-ttu-id="7e14e-1554">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7e14e-1555">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-1556">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-1556">IoT</span></span>

* <span data-ttu-id="7e14e-1557">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1558">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1558">Monitor</span></span>

* <span data-ttu-id="7e14e-1559">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1560">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1560">Network</span></span>

* <span data-ttu-id="7e14e-1561">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7e14e-1562">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7e14e-1563">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7e14e-1564">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7e14e-1565">예약</span><span class="sxs-lookup"><span data-stu-id="7e14e-1565">Reservations</span></span>

* <span data-ttu-id="7e14e-1566">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1567">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1567">Resource</span></span>

* <span data-ttu-id="7e14e-1568">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1569">SQL</span></span>

* <span data-ttu-id="7e14e-1570">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1571">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1571">Storage</span></span>

* <span data-ttu-id="7e14e-1572">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7e14e-1573">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7e14e-1574">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7e14e-1575">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="7e14e-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7e14e-1576">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7e14e-1577">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7e14e-1578">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1579">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1579">VM</span></span>

* <span data-ttu-id="7e14e-1580">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7e14e-1581">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7e14e-1582">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7e14e-1583">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7e14e-1584">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7e14e-1585">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1585">October 24, 2017</span></span>

<span data-ttu-id="7e14e-1586">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7e14e-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1587">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1587">Core</span></span>

* <span data-ttu-id="7e14e-1588">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1589">ACR</span></span>

* <span data-ttu-id="7e14e-1590">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7e14e-1591">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7e14e-1592">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1593">ACS</span></span>

* <span data-ttu-id="7e14e-1594">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7e14e-1595">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1596">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1596">Appservice</span></span>

* <span data-ttu-id="7e14e-1597">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7e14e-1598">구성 요소</span><span class="sxs-lookup"><span data-stu-id="7e14e-1598">Component</span></span>

* <span data-ttu-id="7e14e-1599">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1600">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1600">Monitor</span></span>

* <span data-ttu-id="7e14e-1601">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1602">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1602">Resource</span></span>

* <span data-ttu-id="7e14e-1603">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7e14e-1604">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1605">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1605">VM</span></span>

* <span data-ttu-id="7e14e-1606">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7e14e-1607">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1607">October 9, 2017</span></span>

<span data-ttu-id="7e14e-1608">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7e14e-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1609">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1609">Core</span></span>

* <span data-ttu-id="7e14e-1610">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1611">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1611">Appservice</span></span>

* <span data-ttu-id="7e14e-1612">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-1613">Batch</span></span>

* <span data-ttu-id="7e14e-1614">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7e14e-1615">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7e14e-1616">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7e14e-1617">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7e14e-1618">Batchai</span><span class="sxs-lookup"><span data-stu-id="7e14e-1618">Batchai</span></span>

* <span data-ttu-id="7e14e-1619">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-1620">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7e14e-1620">Keyvault</span></span>

* <span data-ttu-id="7e14e-1621">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7e14e-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7e14e-1623">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1623">Network</span></span>

* <span data-ttu-id="7e14e-1624">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7e14e-1625">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1626">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1626">Resource</span></span>

* <span data-ttu-id="7e14e-1627">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7e14e-1628">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7e14e-1629">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7e14e-1630">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1631">Sql</span><span class="sxs-lookup"><span data-stu-id="7e14e-1631">Sql</span></span>

* <span data-ttu-id="7e14e-1632">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7e14e-1633">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7e14e-1634">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1635">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1635">Storage</span></span>

* <span data-ttu-id="7e14e-1636">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1637">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1637">Vm</span></span>

* <span data-ttu-id="7e14e-1638">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7e14e-1639">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7e14e-1640">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7e14e-1641">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7e14e-1642">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7e14e-1643">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1643">September 22, 2017</span></span>

<span data-ttu-id="7e14e-1644">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="7e14e-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1645">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1645">Resource</span></span>

* <span data-ttu-id="7e14e-1646">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7e14e-1647">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7e14e-1648">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7e14e-1649">[주요 변경 내용] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1650">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1650">Network</span></span>

* <span data-ttu-id="7e14e-1651">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7e14e-1652">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7e14e-1653">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7e14e-1654">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7e14e-1655">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7e14e-1656">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7e14e-1657">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1658">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1658">Storage</span></span>

* <span data-ttu-id="7e14e-1659">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7e14e-1660">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7e14e-1660">Eventgrid</span></span>

* <span data-ttu-id="7e14e-1661">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="7e14e-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1662">SQL</span></span>

* <span data-ttu-id="7e14e-1663">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7e14e-1664">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7e14e-1665">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-1666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7e14e-1666">Keyvault</span></span>

* <span data-ttu-id="7e14e-1667">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1668">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1668">VM</span></span>

* <span data-ttu-id="7e14e-1669">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7e14e-1670">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e14e-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7e14e-1671">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7e14e-1672">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7e14e-1673">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7e14e-1674">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1675">ACS</span></span>

* <span data-ttu-id="7e14e-1676">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1677">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1677">Appservice</span></span>

* <span data-ttu-id="7e14e-1678">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7e14e-1679">Backup</span><span class="sxs-lookup"><span data-stu-id="7e14e-1679">Backup</span></span>

* <span data-ttu-id="7e14e-1680">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7e14e-1681">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1681">September 11, 2017</span></span>

<span data-ttu-id="7e14e-1682">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7e14e-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7e14e-1683">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1683">Core</span></span>

* <span data-ttu-id="7e14e-1684">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7e14e-1685">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1686">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1686">Acs</span></span>

* <span data-ttu-id="7e14e-1687">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7e14e-1688">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1689">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1689">Appservice</span></span>

* <span data-ttu-id="7e14e-1690">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7e14e-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="7e14e-1691">CDN</span></span>

* <span data-ttu-id="7e14e-1692">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7e14e-1693">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7e14e-1693">Extension</span></span>

* <span data-ttu-id="7e14e-1694">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7e14e-1695">Keyvault</span></span>

* <span data-ttu-id="7e14e-1696">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1697">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1697">Network</span></span>

* <span data-ttu-id="7e14e-1698">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7e14e-1699">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7e14e-1700">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7e14e-1701">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7e14e-1702">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1703">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1703">Resource</span></span>

* <span data-ttu-id="7e14e-1704">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7e14e-1705">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7e14e-1706">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7e14e-1707">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="7e14e-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1708">SQL</span></span>

* <span data-ttu-id="7e14e-1709">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1710">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1710">VM</span></span>

* <span data-ttu-id="7e14e-1711">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7e14e-1712">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7e14e-1713">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7e14e-1714">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7e14e-1715">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7e14e-1716">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1716">August 31, 2017</span></span>

<span data-ttu-id="7e14e-1717">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7e14e-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-1718">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7e14e-1718">Keyvault</span></span>

* <span data-ttu-id="7e14e-1719">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7e14e-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="7e14e-1720">Sf</span></span>

* <span data-ttu-id="7e14e-1721">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1722">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1722">Storage</span></span>

* <span data-ttu-id="7e14e-1723">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7e14e-1724">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7e14e-1725">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1725">August 28, 2017</span></span>

<span data-ttu-id="7e14e-1726">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7e14e-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7e14e-1727">CLI</span><span class="sxs-lookup"><span data-stu-id="7e14e-1727">CLI</span></span>

* <span data-ttu-id="7e14e-1728">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1729">ACS</span></span>

* <span data-ttu-id="7e14e-1730">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1730">Corrected preview regions</span></span>
* <span data-ttu-id="7e14e-1731">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7e14e-1732">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1733">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1733">Appservice</span></span>

* <span data-ttu-id="7e14e-1734">[주요 변경 내용] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7e14e-1735">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7e14e-1736">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7e14e-1737">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7e14e-1738">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-1739">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-1739">IoT</span></span>

* <span data-ttu-id="7e14e-1740">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1741">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1741">Network</span></span>

* <span data-ttu-id="7e14e-1742">[주요 변경 내용] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7e14e-1743">[주요 변경 내용] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7e14e-1744">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7e14e-1745">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7e14e-1746">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1747">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1747">Profile</span></span>

* <span data-ttu-id="7e14e-1748">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7e14e-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7e14e-1749">Service Fabric</span></span>

* <span data-ttu-id="7e14e-1750">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1750">Preview release</span></span>
* <span data-ttu-id="7e14e-1751">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7e14e-1752">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7e14e-1753">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1754">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1754">Storage</span></span>

* <span data-ttu-id="7e14e-1755">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="7e14e-1756">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7e14e-1757">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7e14e-1758">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7e14e-1759">[주요 변경 내용] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7e14e-1760">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1761">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1761">VM</span></span>

* <span data-ttu-id="7e14e-1762">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7e14e-1763">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7e14e-1764">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7e14e-1765">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7e14e-1766">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7e14e-1767">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7e14e-1768">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1768">August 15, 2017</span></span>

<span data-ttu-id="7e14e-1769">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7e14e-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1770">ACS</span></span>

* <span data-ttu-id="7e14e-1771">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1772">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1772">Appservice</span></span>

* <span data-ttu-id="7e14e-1773">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7e14e-1774">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7e14e-1774">Event Grid</span></span>

* <span data-ttu-id="7e14e-1775">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7e14e-1776">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1776">August 11, 2017</span></span>

<span data-ttu-id="7e14e-1777">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7e14e-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1778">ACS</span></span>

* <span data-ttu-id="7e14e-1779">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-1780">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-1780">Batch</span></span>

* <span data-ttu-id="7e14e-1781">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7e14e-1782">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7e14e-1783">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7e14e-1784">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7e14e-1785">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7e14e-1786">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7e14e-1787">구성 요소</span><span class="sxs-lookup"><span data-stu-id="7e14e-1787">Component</span></span>

* <span data-ttu-id="7e14e-1788">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7e14e-1789">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7e14e-1789">Container</span></span>

* <span data-ttu-id="7e14e-1790">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7e14e-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7e14e-1791">Data Lake Store</span></span>

* <span data-ttu-id="7e14e-1792">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7e14e-1793">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7e14e-1793">Event Grid</span></span>

* <span data-ttu-id="7e14e-1794">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1795">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1795">Network</span></span>

* <span data-ttu-id="7e14e-1796">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7e14e-1797">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7e14e-1798">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7e14e-1799">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1800">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1800">Profile</span></span>

* <span data-ttu-id="7e14e-1801">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1802">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1802">Storage</span></span>

* <span data-ttu-id="7e14e-1803">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1804">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1804">VM</span></span>

* <span data-ttu-id="7e14e-1805">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7e14e-1806">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7e14e-1807">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7e14e-1808">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7e14e-1809">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7e14e-1810">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1810">July 28, 2017</span></span>

<span data-ttu-id="7e14e-1811">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7e14e-1811">Version 2.0.12</span></span>

* <span data-ttu-id="7e14e-1812">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1812">Added container commands</span></span>
* <span data-ttu-id="7e14e-1813">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7e14e-1814">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-1814">Core</span></span>

* <span data-ttu-id="7e14e-1815">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7e14e-1816">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7e14e-1817">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7e14e-1818">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7e14e-1819">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="7e14e-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7e14e-1820">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7e14e-1821">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7e14e-1822">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7e14e-1823">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7e14e-1824">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7e14e-1825">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="7e14e-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7e14e-1826">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7e14e-1827">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7e14e-1828">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7e14e-1829">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7e14e-1830">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7e14e-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="7e14e-1831">ACR</span></span>

* <span data-ttu-id="7e14e-1832">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7e14e-1833">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7e14e-1834">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7e14e-1835">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7e14e-1836">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7e14e-1837">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1838">ACS</span></span>

* <span data-ttu-id="7e14e-1839">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-1840">App Service</span><span class="sxs-lookup"><span data-stu-id="7e14e-1840">Appservice</span></span>

* <span data-ttu-id="7e14e-1841">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7e14e-1842">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7e14e-1843">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7e14e-1844">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7e14e-1845">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7e14e-1846">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7e14e-1847">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7e14e-1848">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7e14e-1849">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7e14e-1850">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7e14e-1851">Batch</span><span class="sxs-lookup"><span data-stu-id="7e14e-1851">Batch</span></span>

* <span data-ttu-id="7e14e-1852">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7e14e-1853">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7e14e-1854">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7e14e-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="7e14e-1855">CDN</span></span>

* <span data-ttu-id="7e14e-1856">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7e14e-1857">클라우드</span><span class="sxs-lookup"><span data-stu-id="7e14e-1857">Cloud</span></span>

* <span data-ttu-id="7e14e-1858">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7e14e-1859">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7e14e-1860">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7e14e-1861">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7e14e-1862">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-1863">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-1863">CosmosDB</span></span>

* <span data-ttu-id="7e14e-1864">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7e14e-1865">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7e14e-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7e14e-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="7e14e-1867">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7e14e-1868">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7e14e-1869">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7e14e-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7e14e-1870">Data Lake Store</span></span>

* <span data-ttu-id="7e14e-1871">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7e14e-1872">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7e14e-1873">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7e14e-1874">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="7e14e-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7e14e-1875">대화형</span><span class="sxs-lookup"><span data-stu-id="7e14e-1875">Interactive</span></span>

* <span data-ttu-id="7e14e-1876">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7e14e-1877">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1877">Increased test coverage</span></span>
* <span data-ttu-id="7e14e-1878">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7e14e-1879">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7e14e-1880">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7e14e-1881">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7e14e-1882">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7e14e-1883">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="7e14e-1884">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7e14e-1885">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7e14e-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="7e14e-1886">IoT</span></span>

* <span data-ttu-id="7e14e-1887">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7e14e-1888">(#3934)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7e14e-1889">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="7e14e-1889">Key vault</span></span>

* <span data-ttu-id="7e14e-1890">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="7e14e-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7e14e-1891">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7e14e-1892">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7e14e-1893">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7e14e-1894">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7e14e-1895">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7e14e-1896">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7e14e-1897">(#3307)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7e14e-1898">랩</span><span class="sxs-lookup"><span data-stu-id="7e14e-1898">Lab</span></span>

* <span data-ttu-id="7e14e-1899">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7e14e-1900">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-1901">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-1901">Monitor</span></span>

* <span data-ttu-id="7e14e-1902">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7e14e-1903">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7e14e-1904">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7e14e-1905">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7e14e-1906">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7e14e-1907">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7e14e-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7e14e-1908">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7e14e-1909">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7e14e-1910">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1910">`location` no longer required</span></span>
  * <span data-ttu-id="7e14e-1911">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="7e14e-1912">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7e14e-1913">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7e14e-1914">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7e14e-1915">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7e14e-1916">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7e14e-1917">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-1918">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-1918">Network</span></span>

* <span data-ttu-id="7e14e-1919">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7e14e-1920">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7e14e-1921">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7e14e-1922">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7e14e-1923">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7e14e-1924">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7e14e-1925">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7e14e-1926">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7e14e-1927">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7e14e-1928">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7e14e-1929">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7e14e-1930">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7e14e-1931">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7e14e-1932">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7e14e-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7e14e-1933">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7e14e-1934">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7e14e-1935">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7e14e-1936">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7e14e-1937">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7e14e-1938">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7e14e-1939">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7e14e-1940">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7e14e-1941">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7e14e-1942">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7e14e-1943">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7e14e-1944">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7e14e-1945">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-1946">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-1946">Profile</span></span>

* <span data-ttu-id="7e14e-1947">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7e14e-1948">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7e14e-1949">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7e14e-1950">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7e14e-1951">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7e14e-1952">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7e14e-1952">RDBMS</span></span>

* <span data-ttu-id="7e14e-1953">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7e14e-1954">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7e14e-1955">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7e14e-1956">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-1957">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-1957">Resource</span></span>

* <span data-ttu-id="7e14e-1958">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7e14e-1959">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7e14e-1960">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7e14e-1961">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7e14e-1962">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7e14e-1963">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7e14e-1964">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7e14e-1965">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-1966">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-1966">Role</span></span>

* <span data-ttu-id="7e14e-1967">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7e14e-1968">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7e14e-1969">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7e14e-1970">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7e14e-1971">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7e14e-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7e14e-1972">Service Fabric</span></span>
* <span data-ttu-id="7e14e-1973">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="7e14e-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7e14e-1974">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7e14e-1975">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-1976">SQL</span></span>

* <span data-ttu-id="7e14e-1977">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7e14e-1978">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7e14e-1979">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-1980">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-1980">Storage</span></span>

* <span data-ttu-id="7e14e-1981">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7e14e-1982">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="7e14e-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7e14e-1983">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7e14e-1984">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7e14e-1985">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7e14e-1986">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="7e14e-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-1987">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-1987">VM</span></span>

* <span data-ttu-id="7e14e-1988">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1988">Support configuring nsg</span></span>
* <span data-ttu-id="7e14e-1989">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7e14e-1990">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1990">Support managed service identities</span></span>
* <span data-ttu-id="7e14e-1991">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7e14e-1992">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7e14e-1993">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="7e14e-1993">May 10, 2017</span></span>

<span data-ttu-id="7e14e-1994">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7e14e-1994">Version 2.0.6</span></span>

* <span data-ttu-id="7e14e-1995">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="7e14e-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7e14e-1996">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7e14e-1997">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7e14e-1998">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="7e14e-1999">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7e14e-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="7e14e-2000">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="7e14e-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7e14e-2001">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="7e14e-2002">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-2002">Remove Container module</span></span>
* <span data-ttu-id="7e14e-2003">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7e14e-2004">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7e14e-2005">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-2005">Core</span></span>

* <span data-ttu-id="7e14e-2006">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="7e14e-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7e14e-2007">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7e14e-2008">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7e14e-2009">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7e14e-2010">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7e14e-2011">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7e14e-2012">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7e14e-2013">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7e14e-2014">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7e14e-2015">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="7e14e-2015">core: Improved performance</span></span>
* <span data-ttu-id="7e14e-2016">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7e14e-2017">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="7e14e-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-2018">ACS</span></span>

* <span data-ttu-id="7e14e-2019">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7e14e-2020">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="7e14e-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7e14e-2021">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="7e14e-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7e14e-2022">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-2023">AppService</span></span>

* <span data-ttu-id="7e14e-2024">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="7e14e-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7e14e-2025">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7e14e-2026">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="7e14e-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7e14e-2027">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="7e14e-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7e14e-2028">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="7e14e-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7e14e-2029">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7e14e-2030">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-2030">support slot swap with preview</span></span>
* <span data-ttu-id="7e14e-2031">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7e14e-2032">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7e14e-2033">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-2033">CosmosDB</span></span>

* <span data-ttu-id="7e14e-2034">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="7e14e-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7e14e-2035">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7e14e-2036">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7e14e-2037">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7e14e-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7e14e-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="7e14e-2039">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7e14e-2040">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7e14e-2041">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="7e14e-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7e14e-2042">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="7e14e-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7e14e-2043">테이블</span><span class="sxs-lookup"><span data-stu-id="7e14e-2043">Table</span></span>
  * <span data-ttu-id="7e14e-2044">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="7e14e-2044">Table valued function</span></span>
  * <span data-ttu-id="7e14e-2045">보기</span><span class="sxs-lookup"><span data-stu-id="7e14e-2045">View</span></span>
  * <span data-ttu-id="7e14e-2046">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2046">Table Statistics.</span></span> <span data-ttu-id="7e14e-2047">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="7e14e-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7e14e-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7e14e-2048">Data Lake Store</span></span>

* <span data-ttu-id="7e14e-2049">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="7e14e-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7e14e-2050">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7e14e-2051">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2051">missed help for access show.</span></span> <span data-ttu-id="7e14e-2052">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2052">adding it.</span></span> <span data-ttu-id="7e14e-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7e14e-2054">찾기</span><span class="sxs-lookup"><span data-stu-id="7e14e-2054">Find</span></span>

* <span data-ttu-id="7e14e-2055">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="7e14e-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7e14e-2056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7e14e-2056">KeyVault</span></span>

* <span data-ttu-id="7e14e-2057">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7e14e-2058">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="7e14e-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7e14e-2059">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7e14e-2060">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7e14e-2061">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7e14e-2062">랩</span><span class="sxs-lookup"><span data-stu-id="7e14e-2062">Lab</span></span>

* <span data-ttu-id="7e14e-2063">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7e14e-2064">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7e14e-2065">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="7e14e-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7e14e-2066">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="7e14e-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7e14e-2067">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7e14e-2068">모니터</span><span class="sxs-lookup"><span data-stu-id="7e14e-2068">Monitor</span></span>

* <span data-ttu-id="7e14e-2069">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7e14e-2070">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7e14e-2071">네트워크</span><span class="sxs-lookup"><span data-stu-id="7e14e-2071">Network</span></span>

* <span data-ttu-id="7e14e-2072">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7e14e-2073">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7e14e-2074">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7e14e-2075">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7e14e-2076">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7e14e-2077">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7e14e-2078">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7e14e-2079">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7e14e-2080">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7e14e-2081">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7e14e-2082">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="7e14e-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7e14e-2083">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7e14e-2084">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7e14e-2085">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7e14e-2086">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7e14e-2087">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7e14e-2088">프로필</span><span class="sxs-lookup"><span data-stu-id="7e14e-2088">Profile</span></span>

* <span data-ttu-id="7e14e-2089">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7e14e-2090">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7e14e-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="7e14e-2091">Redis</span></span>

* <span data-ttu-id="7e14e-2092">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7e14e-2093">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="7e14e-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7e14e-2094">리소스</span><span class="sxs-lookup"><span data-stu-id="7e14e-2094">Resource</span></span>

* <span data-ttu-id="7e14e-2095">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7e14e-2096">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7e14e-2097">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7e14e-2098">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7e14e-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7e14e-2100">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2100">Add docs for az lock update.</span></span> <span data-ttu-id="7e14e-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7e14e-2102">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7e14e-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7e14e-2104">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7e14e-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7e14e-2106">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7e14e-2107">역할</span><span class="sxs-lookup"><span data-stu-id="7e14e-2107">Role</span></span>

* <span data-ttu-id="7e14e-2108">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7e14e-2109">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7e14e-2110">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7e14e-2111">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="7e14e-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7e14e-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="7e14e-2112">SQL</span></span>

* <span data-ttu-id="7e14e-2113">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7e14e-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7e14e-2114">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7e14e-2115">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-2115">Storage</span></span>

* <span data-ttu-id="7e14e-2116">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="7e14e-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7e14e-2117">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7e14e-2118">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="7e14e-2119">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="7e14e-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-2120">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-2120">VM</span></span>

* <span data-ttu-id="7e14e-2121">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="7e14e-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7e14e-2122">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7e14e-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7e14e-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7e14e-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7e14e-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7e14e-2125">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7e14e-2126">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="7e14e-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7e14e-2127">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7e14e-2128">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="7e14e-2128">April 3, 2017</span></span>

<span data-ttu-id="7e14e-2129">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7e14e-2129">Version 2.0.2</span></span>

<span data-ttu-id="7e14e-2130">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="7e14e-2131">코어</span><span class="sxs-lookup"><span data-stu-id="7e14e-2131">Core</span></span>

* <span data-ttu-id="7e14e-2132">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="7e14e-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7e14e-2133">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7e14e-2134">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7e14e-2135">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7e14e-2136">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7e14e-2137">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7e14e-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7e14e-2139">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7e14e-2140">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="7e14e-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7e14e-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="7e14e-2141">ACS</span></span>

* <span data-ttu-id="7e14e-2142">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7e14e-2143">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7e14e-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7e14e-2145">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2145">Add support for windows clusters.</span></span> <span data-ttu-id="7e14e-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7e14e-2147">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7e14e-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7e14e-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="7e14e-2149">AppService</span></span>

* <span data-ttu-id="7e14e-2150">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7e14e-2151">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7e14e-2152">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7e14e-2153">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7e14e-2154">DataLake</span><span class="sxs-lookup"><span data-stu-id="7e14e-2154">DataLake</span></span>

* <span data-ttu-id="7e14e-2155">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7e14e-2156">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7e14e-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7e14e-2157">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="7e14e-2157">DocuemntDB</span></span>

* <span data-ttu-id="7e14e-2158">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7e14e-2159">VM</span><span class="sxs-lookup"><span data-stu-id="7e14e-2159">VM</span></span>

* <span data-ttu-id="7e14e-2160">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7e14e-2161">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7e14e-2162">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7e14e-2163">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7e14e-2164">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7e14e-2165">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7e14e-2166">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7e14e-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7e14e-2167">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="7e14e-2167">February 27, 2017</span></span>

<span data-ttu-id="7e14e-2168">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7e14e-2168">Version 2.0.0</span></span>

<span data-ttu-id="7e14e-2169">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7e14e-2170">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="7e14e-2170">Container Service (acs)</span></span>
- <span data-ttu-id="7e14e-2171">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="7e14e-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7e14e-2172">네트워킹</span><span class="sxs-lookup"><span data-stu-id="7e14e-2172">Networking</span></span>
- <span data-ttu-id="7e14e-2173">Storage</span><span class="sxs-lookup"><span data-stu-id="7e14e-2173">Storage</span></span>

<span data-ttu-id="7e14e-2174">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7e14e-2175">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7e14e-2176">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="7e14e-2177">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7e14e-2178">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7e14e-2179">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e14e-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7e14e-2180">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="7e14e-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7e14e-2181">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="7e14e-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7e14e-2182">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="7e14e-2182">Provide feedback from the command line with the `az feedback` command</span></span>


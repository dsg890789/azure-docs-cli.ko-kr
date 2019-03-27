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
ms.openlocfilehash: 4337f2203841d6247e4b487d245138424c63e448
ms.sourcegitcommit: 71c0ccd475524cf4d6db45bba8139fef3262d764
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2019
ms.locfileid: "58175136"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="41388-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="41388-103">Azure CLI release notes</span></span>
## <a name="march-12-2019"></a><span data-ttu-id="41388-104">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="41388-104">March 12, 2019</span></span>

<span data-ttu-id="41388-105">2.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="41388-105">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="41388-106">코어</span><span class="sxs-lookup"><span data-stu-id="41388-106">Core</span></span>

* <span data-ttu-id="41388-107">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="41388-107">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="41388-108">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-108">ACR</span></span>

* <span data-ttu-id="41388-109">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="41388-109">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="41388-110">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-110">ACS</span></span>

* <span data-ttu-id="41388-111">`kubectl`이 지원하지 않는 경우 `--listen-address` 인수를 `aks browse`로 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-111">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-112">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-112">AppService</span></span>

* <span data-ttu-id="41388-113">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-113">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="41388-114">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="41388-114">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="41388-115">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-115">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="41388-116">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="41388-116">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="41388-117">Botservice</span><span class="sxs-lookup"><span data-stu-id="41388-117">Botservice</span></span>

* <span data-ttu-id="41388-118">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="41388-118">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="41388-119">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-119">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="41388-120">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="41388-120">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="41388-121">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-121">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="41388-122">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-122">Container</span></span>

* <span data-ttu-id="41388-123">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-123">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="41388-124">EventHub</span><span class="sxs-lookup"><span data-stu-id="41388-124">EventHub</span></span>

* <span data-ttu-id="41388-125">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-125">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="41388-126">찾기</span><span class="sxs-lookup"><span data-stu-id="41388-126">Find</span></span>

* <span data-ttu-id="41388-127">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-127">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="41388-128">HDInsight</span><span class="sxs-lookup"><span data-stu-id="41388-128">HDInsight</span></span>

* <span data-ttu-id="41388-129">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-129">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="41388-130">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-130">Network</span></span>

* <span data-ttu-id="41388-131">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-131">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-132">Rdbms</span><span class="sxs-lookup"><span data-stu-id="41388-132">Rdbms</span></span>

* <span data-ttu-id="41388-133">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="41388-133">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="41388-134">역할</span><span class="sxs-lookup"><span data-stu-id="41388-134">Role</span></span>

* <span data-ttu-id="41388-135">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-135">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="41388-136">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-136">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="41388-137">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="41388-137">Service Fabric</span></span>

* <span data-ttu-id="41388-138">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-138">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="41388-139">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="41388-139">February 26, 2019</span></span>

<span data-ttu-id="41388-140">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="41388-140">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="41388-141">코어</span><span class="sxs-lookup"><span data-stu-id="41388-141">Core</span></span>

* <span data-ttu-id="41388-142">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-142">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="41388-143">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-143">ACR</span></span>

* <span data-ttu-id="41388-144">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-144">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="41388-145">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="41388-145">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="41388-146">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-146">ACS</span></span>

* <span data-ttu-id="41388-147">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-147">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-148">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-148">AppService</span></span>

* <span data-ttu-id="41388-149">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-149">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="41388-150">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-150">Batch</span></span>
* <span data-ttu-id="41388-151">[주요 변경 내용] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-151">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="41388-152">[주요 변경 내용] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-152">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="41388-153">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-153">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="41388-154">[주요 변경 내용] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-154">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="41388-155">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-155">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="41388-156">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-156">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-157">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-157">CosmosDB</span></span>

* <span data-ttu-id="41388-158">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-158">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="41388-159">Kusto</span><span class="sxs-lookup"><span data-stu-id="41388-159">Kusto</span></span>

* <span data-ttu-id="41388-160">[주요 변경 내용] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-160">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="41388-161">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-161">Network</span></span>

* <span data-ttu-id="41388-162">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-162">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="41388-163">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-163">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="41388-164">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-164">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="41388-165">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="41388-165">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="41388-166">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-166">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="41388-167">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-167">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="41388-168">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-168">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="41388-169">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-169">Resource</span></span>

* <span data-ttu-id="41388-170">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-170">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="41388-171">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-171">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="41388-172">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-172">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="41388-173">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="41388-173">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="41388-174">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-174">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="41388-175">역할</span><span class="sxs-lookup"><span data-stu-id="41388-175">Role</span></span>

* <span data-ttu-id="41388-176">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-176">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-177">VM</span><span class="sxs-lookup"><span data-stu-id="41388-177">VM</span></span>

* <span data-ttu-id="41388-178">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-178">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="41388-179">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="41388-179">February 12, 2019</span></span>

<span data-ttu-id="41388-180">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="41388-180">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="41388-181">코어</span><span class="sxs-lookup"><span data-stu-id="41388-181">Core</span></span>

* <span data-ttu-id="41388-182">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-182">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="41388-183">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-183">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="41388-184">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-184">ACR</span></span>
* <span data-ttu-id="41388-185">[주요 변경 내용] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-185">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="41388-186">[주요 변경 내용] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-186">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="41388-187">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-187">ACS</span></span>
* <span data-ttu-id="41388-188">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-188">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="41388-189">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-189">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="41388-190">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-190">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="41388-191">AMS</span><span class="sxs-lookup"><span data-stu-id="41388-191">AMS</span></span>
* <span data-ttu-id="41388-192">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-192">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="41388-193">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-193">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-194">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-194">Appservice</span></span>
* <span data-ttu-id="41388-195">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-195">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="41388-196">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-196">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="41388-197">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-197">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="41388-198">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-198">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="41388-199">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-199">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="41388-200">Botservice</span><span class="sxs-lookup"><span data-stu-id="41388-200">Botservice</span></span>
* <span data-ttu-id="41388-201">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-201">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="41388-202">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-202">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="41388-203">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-203">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="41388-204">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-204">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="41388-205">[사용되지 않음] `--proj-name` 인수가 `--proj-file-path`를 위해 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-205">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="41388-206">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-206">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="41388-207">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-207">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="41388-208">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-208">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="41388-209">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="41388-209">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="41388-210">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-210">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="41388-211">Key Vault</span><span class="sxs-lookup"><span data-stu-id="41388-211">Key Vault</span></span>
* <span data-ttu-id="41388-212">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-212">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-213">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-213">Monitor</span></span>
* <span data-ttu-id="41388-214">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-214">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="41388-215">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-215">Network</span></span>
* <span data-ttu-id="41388-216">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-216">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="41388-217">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-217">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="41388-218">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-218">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="41388-219">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-219">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="41388-220">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="41388-220">Policy Insights</span></span>
* <span data-ttu-id="41388-221">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-221">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-222">RDBMS</span></span>
* <span data-ttu-id="41388-223">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-223">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="41388-224">Redis</span><span class="sxs-lookup"><span data-stu-id="41388-224">Redis</span></span>
* <span data-ttu-id="41388-225">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-225">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="41388-226">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-226">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="41388-227">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-227">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="41388-228">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-228">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="41388-229">[주요 변경 내용] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-229">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="41388-230">[주요 변경 내용] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-230">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="41388-231">[사용되지 않음] `redis import-method` 명령의 사용 중단에 대한 경고 메시지가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-231">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="41388-232">역할</span><span class="sxs-lookup"><span data-stu-id="41388-232">Role</span></span>
* <span data-ttu-id="41388-233">[주요 변경 내용] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-233">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="41388-234">SQL VM</span><span class="sxs-lookup"><span data-stu-id="41388-234">SQL VM</span></span>
* <span data-ttu-id="41388-235">[사용되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-235">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="41388-236">VM</span><span class="sxs-lookup"><span data-stu-id="41388-236">VM</span></span>
* <span data-ttu-id="41388-237">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-237">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="41388-238">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-238">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="41388-239">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-239">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="41388-240">[주요 변경 내용] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-240">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="41388-241">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="41388-241">January 31, 2019</span></span>

<span data-ttu-id="41388-242">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="41388-242">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="41388-243">코어</span><span class="sxs-lookup"><span data-stu-id="41388-243">Core</span></span>

* <span data-ttu-id="41388-244">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="41388-244">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="41388-245">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="41388-245">January 28, 2019</span></span>

<span data-ttu-id="41388-246">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="41388-246">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="41388-247">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-247">ACR</span></span>
* <span data-ttu-id="41388-248">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-248">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="41388-249">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-249">ACS</span></span>
* <span data-ttu-id="41388-250">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="41388-250">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="41388-251">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-251">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="41388-252">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-252">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="41388-253">AMS</span><span class="sxs-lookup"><span data-stu-id="41388-253">AMS</span></span>
* <span data-ttu-id="41388-254">[주요 변경 내용] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-254">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="41388-255">[주요 변경 내용] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-255">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-256">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-256">Appservice</span></span>
* <span data-ttu-id="41388-257">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-257">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="41388-258">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 Function Apps에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-258">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="41388-259">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-259">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="41388-260">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-260">Container</span></span>
* <span data-ttu-id="41388-261">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-261">Added `container start` command</span></span>
* <span data-ttu-id="41388-262">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-262">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="41388-263">EventGrid</span><span class="sxs-lookup"><span data-stu-id="41388-263">EventGrid</span></span>
* <span data-ttu-id="41388-264">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-264">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="41388-265">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-265">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="41388-266">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-266">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="41388-267">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-267">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="41388-268">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-268">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="41388-269">HDInsight</span><span class="sxs-lookup"><span data-stu-id="41388-269">HDInsight</span></span>
* <span data-ttu-id="41388-270">[주요 변경 내용] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-270">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="41388-271">[주요 변경 내용] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-271">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="41388-272">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-272">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="41388-273">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-273">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="41388-274">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-274">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="41388-275">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-275">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="41388-276">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-276">IoT</span></span>
* <span data-ttu-id="41388-277">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-277">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="41388-278">Kusto</span><span class="sxs-lookup"><span data-stu-id="41388-278">Kusto</span></span>
* <span data-ttu-id="41388-279">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-279">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-280">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-280">Monitor</span></span>
* <span data-ttu-id="41388-281">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-281">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="41388-282">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-282">Profile</span></span>
* <span data-ttu-id="41388-283">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-283">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="41388-284">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-284">Network</span></span>
* <span data-ttu-id="41388-285">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-285">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="41388-286">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-286">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="41388-287">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-287">Resource</span></span>
* <span data-ttu-id="41388-288">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-288">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="41388-289">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-289">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="41388-290">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="41388-290">SQL Virtual Machine</span></span>
* <span data-ttu-id="41388-291">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-291">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="41388-292">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-292">Storage</span></span>
* <span data-ttu-id="41388-293">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-293">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="41388-294">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-294">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="41388-295">VM</span><span class="sxs-lookup"><span data-stu-id="41388-295">VM</span></span>
* <span data-ttu-id="41388-296">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-296">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="41388-297">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-297">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="41388-298">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="41388-298">January 15, 2019</span></span>

<span data-ttu-id="41388-299">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="41388-299">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="41388-300">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-300">ACR</span></span>
* <span data-ttu-id="41388-301">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-301">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="41388-302">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-302">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="41388-303">[사용되지 않음] `--resource-group` 매개 변수가 다음 명령에서 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-303">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="41388-304">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-304">ACS</span></span>
* <span data-ttu-id="41388-305">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-305">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-306">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-306">Appservice</span></span>
* <span data-ttu-id="41388-307">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-307">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="41388-308">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-308">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="41388-309">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-309">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="41388-310">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-310">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="41388-311">Botservice</span><span class="sxs-lookup"><span data-stu-id="41388-311">Botservice</span></span>
* <span data-ttu-id="41388-312">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-312">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="41388-313">구성</span><span class="sxs-lookup"><span data-stu-id="41388-313">Configure</span></span>
* <span data-ttu-id="41388-314">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-314">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-315">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-315">CosmosDB</span></span>
* <span data-ttu-id="41388-316">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-316">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="41388-317">HDInsight</span><span class="sxs-lookup"><span data-stu-id="41388-317">HDInsight</span></span>
* <span data-ttu-id="41388-318">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-318">Added commands for managing applications</span></span>
* <span data-ttu-id="41388-319">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-319">Added commands for managing script actions</span></span>
* <span data-ttu-id="41388-320">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-320">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="41388-321">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-321">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="41388-322">[주요 변경 내용] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-322">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="41388-323">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-323">Network</span></span>
* <span data-ttu-id="41388-324">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-324">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="41388-325">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-325">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="41388-326">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-326">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="41388-327">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-327">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="41388-328">역할</span><span class="sxs-lookup"><span data-stu-id="41388-328">Role</span></span>
* <span data-ttu-id="41388-329">[사용되지 않음] `--password` 인수가 `create-for-rbac`에 대해 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-329">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="41388-330">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-330">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="41388-331">보안</span><span class="sxs-lookup"><span data-stu-id="41388-331">Security</span></span>
* <span data-ttu-id="41388-332">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-332">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="41388-333">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-333">Storage</span></span>
* <span data-ttu-id="41388-334">[주요 변경 내용] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-334">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="41388-335">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-335">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="41388-336">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-336">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="41388-337">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-337">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="41388-338">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-338">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="41388-339">VM</span><span class="sxs-lookup"><span data-stu-id="41388-339">VM</span></span>
* <span data-ttu-id="41388-340">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-340">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="41388-341">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-341">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="41388-342">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-342">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="41388-343">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-343">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="41388-344">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-344">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="41388-345">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-345">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="41388-346">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="41388-346">December 20, 2018</span></span>

<span data-ttu-id="41388-347">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="41388-347">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="41388-348">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-348">Appservice</span></span>
* <span data-ttu-id="41388-349">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-349">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="41388-350">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-350">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="41388-351">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-351">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="41388-352">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="41388-352">IoTCentral</span></span>
* <span data-ttu-id="41388-353">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-353">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="41388-354">역할</span><span class="sxs-lookup"><span data-stu-id="41388-354">Role</span></span>
* <span data-ttu-id="41388-355">[주요 변경 내용] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-355">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="41388-356">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-356">SQL</span></span>
* <span data-ttu-id="41388-357">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-357">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="41388-358">VM</span><span class="sxs-lookup"><span data-stu-id="41388-358">VM</span></span>
* <span data-ttu-id="41388-359">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-359">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="41388-360">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="41388-360">December 18, 2018</span></span>

<span data-ttu-id="41388-361">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="41388-361">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="41388-362">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-362">ACR</span></span>
* <span data-ttu-id="41388-363">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-363">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="41388-364">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="41388-364">Condensed the table layout for task list</span></span>
* <span data-ttu-id="41388-365">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-365">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="41388-366">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-366">ACS</span></span>
* <span data-ttu-id="41388-367">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="41388-367">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="41388-368">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="41388-368">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="41388-369">[사용되지 않음] `az acs` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-369">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="41388-370">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-370">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="41388-371">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-371">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="41388-372">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="41388-372">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-373">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-373">Appservice</span></span>
* <span data-ttu-id="41388-374">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="41388-374">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="41388-375">Botservice</span><span class="sxs-lookup"><span data-stu-id="41388-375">Botservice</span></span>
* <span data-ttu-id="41388-376">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-376">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="41388-377">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="41388-377">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="41388-378">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="41388-378">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="41388-379">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="41388-379">Reduced Kudu network calls</span></span>
* <span data-ttu-id="41388-380">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="41388-380">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-381">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-381">Consumption</span></span>
* <span data-ttu-id="41388-382">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-382">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-383">CosmosDB</span></span>
* <span data-ttu-id="41388-384">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-384">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="41388-385">지도</span><span class="sxs-lookup"><span data-stu-id="41388-385">Maps</span></span>
* <span data-ttu-id="41388-386">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-386">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="41388-387">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-387">Network</span></span>
* <span data-ttu-id="41388-388">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-388">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="41388-389">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="41388-389">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="41388-390">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-390">Resource</span></span>
* <span data-ttu-id="41388-391">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-391">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="41388-392">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-392">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-393">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-393">Storage</span></span>
*  <span data-ttu-id="41388-394">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-394">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-395">VM</span><span class="sxs-lookup"><span data-stu-id="41388-395">VM</span></span>
* <span data-ttu-id="41388-396">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-396">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="41388-397">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="41388-397">December 4, 2018</span></span>

<span data-ttu-id="41388-398">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="41388-398">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="41388-399">코어</span><span class="sxs-lookup"><span data-stu-id="41388-399">Core</span></span>
* <span data-ttu-id="41388-400">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-400">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="41388-401">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-401">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-402">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-402">Appservice</span></span>
* <span data-ttu-id="41388-403">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-403">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="41388-404">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-404">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="41388-405">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-405">Network</span></span>
* <span data-ttu-id="41388-406">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-406">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="41388-407">역할</span><span class="sxs-lookup"><span data-stu-id="41388-407">Role</span></span>
* <span data-ttu-id="41388-408">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-408">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="41388-409">VM</span><span class="sxs-lookup"><span data-stu-id="41388-409">VM</span></span>
* <span data-ttu-id="41388-410">[사용되지 않음]`vm extension [show|wait] --expand` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-410">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="41388-411">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-411">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="41388-412">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-412">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="41388-413">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-413">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="41388-414">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="41388-414">November 20, 2018</span></span>

<span data-ttu-id="41388-415">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="41388-415">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="41388-416">코어</span><span class="sxs-lookup"><span data-stu-id="41388-416">Core</span></span>
* <span data-ttu-id="41388-417">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="41388-417">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="41388-418">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-418">ACR</span></span>
* <span data-ttu-id="41388-419">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="41388-419">Added context token to task step</span></span>
* <span data-ttu-id="41388-420">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-420">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="41388-421">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="41388-421">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-422">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-422">Appservice</span></span>
* <span data-ttu-id="41388-423">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-423">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="41388-424">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-424">Updated the default `node_version`.</span></span> <span data-ttu-id="41388-425">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-425">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="41388-426">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="41388-426">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="41388-427">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-427">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="41388-428">IotCentral</span><span class="sxs-lookup"><span data-stu-id="41388-428">IotCentral</span></span>
* <span data-ttu-id="41388-429">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="41388-429">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-430">KeyVault</span><span class="sxs-lookup"><span data-stu-id="41388-430">KeyVault</span></span>
* <span data-ttu-id="41388-431">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-431">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="41388-432">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-432">Network</span></span>
* <span data-ttu-id="41388-433">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-433">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="41388-434">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="41388-434">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="41388-435">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-435">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="41388-436">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="41388-436">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-437">Rdbms</span><span class="sxs-lookup"><span data-stu-id="41388-437">Rdbms</span></span>
* <span data-ttu-id="41388-438">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-438">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="41388-439">Rbac</span><span class="sxs-lookup"><span data-stu-id="41388-439">Rbac</span></span>
* <span data-ttu-id="41388-440">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-440">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="41388-441">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-441">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="41388-442">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-442">Storage</span></span>
* <span data-ttu-id="41388-443">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-443">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="41388-444">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-444">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="41388-445">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-445">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="41388-446">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-446">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="41388-447">VM</span><span class="sxs-lookup"><span data-stu-id="41388-447">VM</span></span>
* <span data-ttu-id="41388-448">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-448">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="41388-449">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-449">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="41388-450">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="41388-450">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="41388-451">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-451">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="41388-452">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-452">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="41388-453">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-453">Added `snapshot wait` command</span></span>
* <span data-ttu-id="41388-454">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-454">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="41388-455">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="41388-455">November 6, 2018</span></span>

<span data-ttu-id="41388-456">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="41388-456">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="41388-457">코어</span><span class="sxs-lookup"><span data-stu-id="41388-457">Core</span></span>
* <span data-ttu-id="41388-458">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-458">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="41388-459">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-459">ACR</span></span>
* <span data-ttu-id="41388-460">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-460">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="41388-461">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-461">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="41388-462">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-462">ACS</span></span>
* <span data-ttu-id="41388-463">[주요 변경 내용] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-463">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="41388-464">Advisor</span><span class="sxs-lookup"><span data-stu-id="41388-464">Advisor</span></span>
* <span data-ttu-id="41388-465">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-465">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="41388-466">AMS</span><span class="sxs-lookup"><span data-stu-id="41388-466">AMS</span></span>
* <span data-ttu-id="41388-467">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="41388-467">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="41388-468">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="41388-468">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="41388-469">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-469">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="41388-470">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="41388-470">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="41388-471">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-471">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="41388-472">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-472">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="41388-473">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-473">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="41388-474">[주요 변경 내용] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="41388-474">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="41388-475">[주요 변경 내용] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-475">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="41388-476">[주요 변경 내용] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-476">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="41388-477">[주요 변경 내용] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="41388-477">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="41388-478">[주요 변경 내용] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="41388-478">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="41388-479">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="41388-479">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="41388-480">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="41388-480">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="41388-481">[주요 변경 내용] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-481">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="41388-482">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-482">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="41388-483">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-483">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-484">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-484">AppService</span></span>
* <span data-ttu-id="41388-485">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-485">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="41388-486">구성</span><span class="sxs-lookup"><span data-stu-id="41388-486">Configure</span></span>
* <span data-ttu-id="41388-487">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-487">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="41388-488">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-488">Container</span></span>
* <span data-ttu-id="41388-489">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-489">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="41388-490">EventHub</span><span class="sxs-lookup"><span data-stu-id="41388-490">EventHub</span></span>
* <span data-ttu-id="41388-491">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-491">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-492">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-492">Interactive</span></span>
* <span data-ttu-id="41388-493">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="41388-493">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-494">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-494">Monitor</span></span>
* <span data-ttu-id="41388-495">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-495">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="41388-496">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-496">Network</span></span>
* <span data-ttu-id="41388-497">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-497">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="41388-498">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-498">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="41388-499">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-499">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="41388-500">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-500">Profile</span></span>
* <span data-ttu-id="41388-501">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-501">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-502">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-502">RDBMS</span></span>
* <span data-ttu-id="41388-503">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-503">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="41388-504">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-504">Resource</span></span>
* <span data-ttu-id="41388-505">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-505">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="41388-506">역할</span><span class="sxs-lookup"><span data-stu-id="41388-506">Role</span></span>
* <span data-ttu-id="41388-507">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-507">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="41388-508">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-508">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="41388-509">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-509">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="41388-510">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-510">Storage</span></span>
* <span data-ttu-id="41388-511">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-511">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-512">VM</span><span class="sxs-lookup"><span data-stu-id="41388-512">VM</span></span>
* <span data-ttu-id="41388-513">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-513">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="41388-514">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-514">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="41388-515">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-515">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="41388-516">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-516">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="41388-517">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="41388-517">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="41388-518">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-518">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="41388-519">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="41388-519">October 23, 2018</span></span>

<span data-ttu-id="41388-520">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="41388-520">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="41388-521">코어</span><span class="sxs-lookup"><span data-stu-id="41388-521">Core</span></span>
* <span data-ttu-id="41388-522">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-522">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="41388-523">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-523">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="41388-524">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-524">ACR</span></span>
* <span data-ttu-id="41388-525">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-525">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="41388-526">CDN</span><span class="sxs-lookup"><span data-stu-id="41388-526">CDN</span></span>
* <span data-ttu-id="41388-527">[주요 변경 내용] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-527">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="41388-528">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-528">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="41388-529">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-529">Container</span></span>
* <span data-ttu-id="41388-530">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-530">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="41388-531">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-531">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="41388-532">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-532">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="41388-533">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-533">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="41388-534">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-534">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="41388-535">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-535">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="41388-536">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-536">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-537">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-537">CosmosDB</span></span>
* <span data-ttu-id="41388-538">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-538">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-539">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-539">Interactive</span></span>
* <span data-ttu-id="41388-540">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-540">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="41388-541">IoT Central</span><span class="sxs-lookup"><span data-stu-id="41388-541">IoT Central</span></span>
* <span data-ttu-id="41388-542">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-542">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="41388-543">[주요 변경 내용] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-543">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-544">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-544">Monitor</span></span>
* <span data-ttu-id="41388-545">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="41388-545">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="41388-546">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-546">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="41388-547">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="41388-548">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="41388-549">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-549">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="41388-550">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-550">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="41388-551">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="41388-551">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="41388-552">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-552">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="41388-553">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-553">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="41388-554">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-554">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="41388-555">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-555">Network</span></span>
* <span data-ttu-id="41388-556">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-556">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="41388-557">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-557">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="41388-558">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41388-558">ServiceBus</span></span>
* <span data-ttu-id="41388-559">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-559">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="41388-560">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-560">SQL</span></span>
* <span data-ttu-id="41388-561">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-561">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="41388-562">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-562">Storage</span></span>
* <span data-ttu-id="41388-563">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-563">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="41388-564">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-564">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="41388-565">VM</span><span class="sxs-lookup"><span data-stu-id="41388-565">VM</span></span>
* <span data-ttu-id="41388-566">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-566">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="41388-567">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-567">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="41388-568">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-568">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="41388-569">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="41388-569">October 16, 2018</span></span>

<span data-ttu-id="41388-570">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="41388-570">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="41388-571">VM</span><span class="sxs-lookup"><span data-stu-id="41388-571">VM</span></span>
* <span data-ttu-id="41388-572">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-572">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="41388-573">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="41388-573">October 9, 2018</span></span>

<span data-ttu-id="41388-574">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="41388-574">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="41388-575">코어</span><span class="sxs-lookup"><span data-stu-id="41388-575">Core</span></span>
* <span data-ttu-id="41388-576">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="41388-576">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="41388-577">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-577">ACR</span></span>
* <span data-ttu-id="41388-578">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-578">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="41388-579">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-579">ACS</span></span>
* <span data-ttu-id="41388-580">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="41388-580">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="41388-581">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="41388-581">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="41388-582">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-582">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="41388-583">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="41388-583">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="41388-584">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-584">Container</span></span>
* <span data-ttu-id="41388-585">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-585">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="41388-586">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-586">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="41388-587">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="41388-587">Event Hub</span></span>
* <span data-ttu-id="41388-588">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-588">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="41388-589">[주요 변경 내용] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="41388-589">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="41388-590">확장</span><span class="sxs-lookup"><span data-stu-id="41388-590">Extensions</span></span>
* <span data-ttu-id="41388-591">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-591">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="41388-592">HDInsight</span><span class="sxs-lookup"><span data-stu-id="41388-592">HDInsight</span></span>
* <span data-ttu-id="41388-593">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-593">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="41388-594">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-594">IoT</span></span>
* <span data-ttu-id="41388-595">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-595">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-596">KeyVault</span><span class="sxs-lookup"><span data-stu-id="41388-596">KeyVault</span></span>
* <span data-ttu-id="41388-597">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-597">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="41388-598">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-598">Network</span></span>
* <span data-ttu-id="41388-599">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-599">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="41388-600">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="41388-600">See #6052</span></span>
* <span data-ttu-id="41388-601">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="41388-601">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="41388-602">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-602">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="41388-603">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-603">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="41388-604">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-604">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="41388-605">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-605">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="41388-606">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-606">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="41388-607">역할</span><span class="sxs-lookup"><span data-stu-id="41388-607">Role</span></span>
* <span data-ttu-id="41388-608">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-608">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="41388-609">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-609">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="41388-610">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-610">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="41388-611">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-611">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="41388-612">Service Bus</span><span class="sxs-lookup"><span data-stu-id="41388-612">Service Bus</span></span>
* <span data-ttu-id="41388-613">[주요 변경 내용] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="41388-613">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="41388-614">VM</span><span class="sxs-lookup"><span data-stu-id="41388-614">VM</span></span>
* <span data-ttu-id="41388-615">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-615">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="41388-616">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-616">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="41388-617">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-617">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="41388-618">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-618">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="41388-619">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-619">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="41388-620">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-620">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="41388-621">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="41388-621">September 21, 2018</span></span>

<span data-ttu-id="41388-622">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="41388-622">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="41388-623">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-623">ACR</span></span>
* <span data-ttu-id="41388-624">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-624">Added ACR Task commands</span></span>
* <span data-ttu-id="41388-625">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-625">Added quick run command</span></span>
* <span data-ttu-id="41388-626">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-626">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="41388-627">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="41388-627">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="41388-628">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-628">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="41388-629">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="41388-629">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="41388-630">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-630">ACS</span></span>
* <span data-ttu-id="41388-631">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="41388-631">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="41388-632">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="41388-632">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-633">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-633">AppService</span></span>

* <span data-ttu-id="41388-634">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-634">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="41388-635">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-635">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="41388-636">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-636">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="41388-637">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-637">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="41388-638">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-638">Batch</span></span>
* <span data-ttu-id="41388-639">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="41388-639">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="41388-640">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-640">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="41388-641">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-641">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="41388-642">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="41388-642">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="41388-643">Batch AI</span><span class="sxs-lookup"><span data-stu-id="41388-643">Batch AI</span></span> 
* <span data-ttu-id="41388-644">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="41388-644">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="41388-645">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="41388-645">Cognitive Services</span></span>
* <span data-ttu-id="41388-646">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="41388-646">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="41388-647">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-647">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="41388-648">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-648">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="41388-649">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-649">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="41388-650">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-650">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="41388-651">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-651">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="41388-652">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-652">Container</span></span>
* <span data-ttu-id="41388-653">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="41388-653">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="41388-654">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-654">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="41388-655">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-655">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="41388-656">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="41388-656">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="41388-657">Datalake</span><span class="sxs-lookup"><span data-stu-id="41388-657">Datalake</span></span>
* <span data-ttu-id="41388-658">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-658">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="41388-659">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="41388-659">Interactive Shell</span></span>
* <span data-ttu-id="41388-660">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="41388-660">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="41388-661">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-661">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="41388-662">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-662">IoT</span></span>
* <span data-ttu-id="41388-663">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-663">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="41388-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="41388-664">Key Vault</span></span>
* <span data-ttu-id="41388-665">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="41388-665">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="41388-666">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-666">Network</span></span>
* <span data-ttu-id="41388-667">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-667">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="41388-668">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-668">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="41388-669">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-669">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="41388-670">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-670">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="41388-671">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-671">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="41388-672">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-672">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="41388-673">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="41388-673">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="41388-674">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-674">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="41388-675">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="41388-675">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="41388-676">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="41388-676">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="41388-677">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-677">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="41388-678">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-678">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="41388-679">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-679">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="41388-680">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하는 논리가 수정됨. 사설 IP 주소가 제공되는 경우 정적 할당이 설정됨. 사설 IP 주소가 제공되지 않는 경우나 사설 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="41388-680">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="41388-681">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-681">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="41388-682">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-682">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="41388-683">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-683">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="41388-684">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-684">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-685">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-685">RDBMS</span></span>
* <span data-ttu-id="41388-686">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-686">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="41388-687">예약</span><span class="sxs-lookup"><span data-stu-id="41388-687">Reservation</span></span>
* <span data-ttu-id="41388-688">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="41388-688">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="41388-689">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="41388-689">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="41388-690">앱 관리</span><span class="sxs-lookup"><span data-stu-id="41388-690">Manage App</span></span>
* <span data-ttu-id="41388-691">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="41388-691">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="41388-692">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="41388-692">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="41388-693">역할</span><span class="sxs-lookup"><span data-stu-id="41388-693">Role</span></span>
* <span data-ttu-id="41388-694">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-694">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="41388-695">SignalR</span><span class="sxs-lookup"><span data-stu-id="41388-695">SignalR</span></span>
* <span data-ttu-id="41388-696">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-696">First release</span></span>

### <a name="storage"></a><span data-ttu-id="41388-697">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-697">Storage</span></span>
* <span data-ttu-id="41388-698">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-698">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="41388-699">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-699">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="41388-700">VM</span><span class="sxs-lookup"><span data-stu-id="41388-700">VM</span></span>
* <span data-ttu-id="41388-701">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="41388-701">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="41388-702">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-702">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="41388-703">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="41388-703">August 28, 2018</span></span>

<span data-ttu-id="41388-704">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="41388-704">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="41388-705">코어</span><span class="sxs-lookup"><span data-stu-id="41388-705">Core</span></span>

* <span data-ttu-id="41388-706">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-706">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="41388-707">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-707">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="41388-708">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-708">ACR</span></span>

* <span data-ttu-id="41388-709">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="41388-709">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="41388-710">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-710">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="41388-711">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-711">ACS</span></span>

* <span data-ttu-id="41388-712">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-712">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="41388-713">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-713">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-714">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-714">AppService</span></span>

* <span data-ttu-id="41388-715">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-715">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="41388-716">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-716">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="41388-717">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-717">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="41388-718">Backup</span><span class="sxs-lookup"><span data-stu-id="41388-718">Backup</span></span>

* <span data-ttu-id="41388-719">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-719">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="41388-720">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="41388-720">Bot Service</span></span>

* <span data-ttu-id="41388-721">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-721">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="41388-722">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="41388-722">Cognitive Services</span></span>

* <span data-ttu-id="41388-723">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-723">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="41388-724">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-724">IoT</span></span>

* <span data-ttu-id="41388-725">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-725">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-726">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-726">Monitor</span></span>

* <span data-ttu-id="41388-727">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-727">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="41388-728">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="41388-728">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="41388-729">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-729">Network</span></span>

* <span data-ttu-id="41388-730">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-730">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="41388-731">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-731">Resource</span></span>

* <span data-ttu-id="41388-732">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-732">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="41388-733">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-733">Storage</span></span>

* <span data-ttu-id="41388-734">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-734">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="41388-735">VM</span><span class="sxs-lookup"><span data-stu-id="41388-735">VM</span></span>

* <span data-ttu-id="41388-736">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-736">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="41388-737">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="41388-737">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="41388-738">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="41388-738">Auguest 14, 2018</span></span>

<span data-ttu-id="41388-739">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="41388-739">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="41388-740">코어</span><span class="sxs-lookup"><span data-stu-id="41388-740">Core</span></span>

* <span data-ttu-id="41388-741">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="41388-741">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="41388-742">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="41388-742">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="41388-743">원격 분석</span><span class="sxs-lookup"><span data-stu-id="41388-743">Telemetry</span></span>

* <span data-ttu-id="41388-744">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="41388-744">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="41388-745">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-745">ACR</span></span>

* <span data-ttu-id="41388-746">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-746">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="41388-747">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-747">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="41388-748">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-748">ACS</span></span>

* <span data-ttu-id="41388-749">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-749">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="41388-750">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-750">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="41388-751">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="41388-751">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="41388-752">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="41388-752">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="41388-753">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-753">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="41388-754">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-754">AppService</span></span>

* <span data-ttu-id="41388-755">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-755">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="41388-756">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="41388-756">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="41388-757">BatchAI</span><span class="sxs-lookup"><span data-stu-id="41388-757">BatchAI</span></span>

* <span data-ttu-id="41388-758">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="41388-758">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="41388-759">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-759">Container</span></span>

* <span data-ttu-id="41388-760">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-760">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="41388-761">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-761">IoT</span></span>

* <span data-ttu-id="41388-762">[주요 변경 내용] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="41388-762">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="41388-763">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-763">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="41388-764">Iot Central</span><span class="sxs-lookup"><span data-stu-id="41388-764">Iot Central</span></span>

* <span data-ttu-id="41388-765">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-765">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-766">KeyVault</span><span class="sxs-lookup"><span data-stu-id="41388-766">KeyVault</span></span>


* <span data-ttu-id="41388-767">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-767">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="41388-768">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-768">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="41388-769">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="41388-769">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="41388-770">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-770">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="41388-771">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-771">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="41388-772">릴레이</span><span class="sxs-lookup"><span data-stu-id="41388-772">Relay</span></span>

* <span data-ttu-id="41388-773">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-773">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="41388-774">Sql</span><span class="sxs-lookup"><span data-stu-id="41388-774">Sql</span></span>

* <span data-ttu-id="41388-775">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-775">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="41388-776">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-776">Storage</span></span>

* <span data-ttu-id="41388-777">[주요 변경 내용] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="41388-777">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="41388-778">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-778">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="41388-779">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="41388-779">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="41388-780">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="41388-780">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="41388-781">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="41388-781">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="41388-782">VM</span><span class="sxs-lookup"><span data-stu-id="41388-782">VM</span></span>

* <span data-ttu-id="41388-783">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-783">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="41388-784">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="41388-784">July 31, 2018</span></span>

<span data-ttu-id="41388-785">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="41388-785">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="41388-786">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-786">ACR</span></span>

* <span data-ttu-id="41388-787">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-787">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="41388-788">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-788">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="41388-789">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-789">ACS</span></span>

* <span data-ttu-id="41388-790">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-790">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="41388-791">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-791">Batch</span></span>

* <span data-ttu-id="41388-792">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-792">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="41388-793">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-793">Container</span></span>

* <span data-ttu-id="41388-794">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-794">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="41388-795">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-795">Network</span></span>

* <span data-ttu-id="41388-796">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-796">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="41388-797">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-797">Resource</span></span>

* <span data-ttu-id="41388-798">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="41388-798">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="41388-799">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="41388-799">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="41388-800">역할</span><span class="sxs-lookup"><span data-stu-id="41388-800">Role</span></span>

* <span data-ttu-id="41388-801">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-801">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="41388-802">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-802">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="41388-803">검색</span><span class="sxs-lookup"><span data-stu-id="41388-803">Search</span></span>

* <span data-ttu-id="41388-804">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-804">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="41388-805">Service Bus</span><span class="sxs-lookup"><span data-stu-id="41388-805">Service Bus</span></span>

* <span data-ttu-id="41388-806">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-806">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="41388-807">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-807">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="41388-808">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="41388-808">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="41388-809">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="41388-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-810">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-810">Storage</span></span>

* <span data-ttu-id="41388-811">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-811">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="41388-812">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="41388-812">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="41388-813">VM</span><span class="sxs-lookup"><span data-stu-id="41388-813">VM</span></span>

* <span data-ttu-id="41388-814">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-814">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="41388-815">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-815">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="41388-816">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-816">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="41388-817">[주요 변경 내용] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-817">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="41388-818">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="41388-818">July 18, 2018</span></span>

<span data-ttu-id="41388-819">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="41388-819">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="41388-820">코어</span><span class="sxs-lookup"><span data-stu-id="41388-820">Core</span></span>

* <span data-ttu-id="41388-821">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-821">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="41388-822">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="41388-822">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="41388-823">[주요 변경 내용] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-823">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="41388-824">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-824">ACR</span></span>

* <span data-ttu-id="41388-825">[주요 변경 내용] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-825">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="41388-826">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-826">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="41388-827">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="41388-827">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="41388-828">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="41388-828">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="41388-829">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-829">ACS</span></span>

* <span data-ttu-id="41388-830">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="41388-830">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-831">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-831">AppService</span></span>

* <span data-ttu-id="41388-832">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-832">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="41388-833">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-833">Batch</span></span>

* <span data-ttu-id="41388-834">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-834">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="41388-835">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-835">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="41388-836">Batch AI</span><span class="sxs-lookup"><span data-stu-id="41388-836">Batch AI</span></span>

* <span data-ttu-id="41388-837">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-837">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="41388-838">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-838">Container</span></span>

* <span data-ttu-id="41388-839">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="41388-839">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="41388-840">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="41388-840">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="41388-841">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-841">Network</span></span>

* <span data-ttu-id="41388-842">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-842">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="41388-843">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-843">Added `network nic wait`</span></span>
* <span data-ttu-id="41388-844">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-844">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="41388-845">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="41388-845">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="41388-846">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-846">Resource</span></span>

* <span data-ttu-id="41388-847">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-847">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="41388-848">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-848">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="41388-849">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-849">Added `deployment wait` command</span></span>
* <span data-ttu-id="41388-850">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-850">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="41388-851">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-851">SQL</span></span>

* <span data-ttu-id="41388-852">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-852">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="41388-853">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="41388-853">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="41388-854">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="41388-854">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="41388-855">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-855">Storage</span></span>

* <span data-ttu-id="41388-856">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="41388-856">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="41388-857">VM</span><span class="sxs-lookup"><span data-stu-id="41388-857">VM</span></span>

* <span data-ttu-id="41388-858">[주요 변경 내용] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-858">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="41388-859">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-859">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="41388-860">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-860">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="41388-861">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="41388-861">July 3, 2018</span></span>

<span data-ttu-id="41388-862">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="41388-862">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="41388-863">AKS</span><span class="sxs-lookup"><span data-stu-id="41388-863">AKS</span></span>

* <span data-ttu-id="41388-864">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="41388-864">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="41388-865">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="41388-865">July 3, 2018</span></span>

<span data-ttu-id="41388-866">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="41388-866">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="41388-867">코어</span><span class="sxs-lookup"><span data-stu-id="41388-867">Core</span></span>

* <span data-ttu-id="41388-868">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="41388-868">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="41388-869">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-869">ACR</span></span>

* <span data-ttu-id="41388-870">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="41388-870">Added polling build status</span></span>
* <span data-ttu-id="41388-871">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-871">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="41388-872">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-872">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="41388-873">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-873">ACS</span></span>

* <span data-ttu-id="41388-874">[주요 변경 내용]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-874">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="41388-875">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-875">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="41388-876">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="41388-876">Updated options for `aks browse` command.</span></span> <span data-ttu-id="41388-877">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-877">Added `--listen-port` support</span></span>
* <span data-ttu-id="41388-878">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="41388-878">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="41388-879">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="41388-879">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="41388-880">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-880">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-881">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-881">AppService</span></span>

* <span data-ttu-id="41388-882">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-882">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="41388-883">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="41388-883">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="41388-884">Backup</span><span class="sxs-lookup"><span data-stu-id="41388-884">Backup</span></span>

* <span data-ttu-id="41388-885">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-885">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="41388-886">BatchAI</span><span class="sxs-lookup"><span data-stu-id="41388-886">BatchAI</span></span>

* <span data-ttu-id="41388-887">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-887">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="41388-888">클라우드</span><span class="sxs-lookup"><span data-stu-id="41388-888">Cloud</span></span>

* <span data-ttu-id="41388-889">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-889">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="41388-890">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-890">Container</span></span>

* <span data-ttu-id="41388-891">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-891">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="41388-892">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-892">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="41388-893">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="41388-893">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="41388-894">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-894">Extension</span></span>

* <span data-ttu-id="41388-895">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-895">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="41388-896">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-896">Network</span></span>

* <span data-ttu-id="41388-897">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="41388-897">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="41388-898">Rdbms</span></span>

* <span data-ttu-id="41388-899">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-899">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="41388-900">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-900">Resource</span></span>

* <span data-ttu-id="41388-901">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-901">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-902">VM</span><span class="sxs-lookup"><span data-stu-id="41388-902">VM</span></span>

* <span data-ttu-id="41388-903">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-903">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="41388-904">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="41388-904">June 25, 2018</span></span>

<span data-ttu-id="41388-905">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="41388-905">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="41388-906">CLI</span><span class="sxs-lookup"><span data-stu-id="41388-906">CLI</span></span>

* <span data-ttu-id="41388-907">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-907">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="41388-908">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="41388-908">June 19, 2018</span></span>

<span data-ttu-id="41388-909">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="41388-909">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="41388-910">코어</span><span class="sxs-lookup"><span data-stu-id="41388-910">Core</span></span>

* <span data-ttu-id="41388-911">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-911">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="41388-912">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-912">ACR</span></span>

* <span data-ttu-id="41388-913">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-913">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="41388-914">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-914">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="41388-915">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-915">ACS</span></span>

* <span data-ttu-id="41388-916">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="41388-916">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="41388-917">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-917">Added `--update` support</span></span>
* <span data-ttu-id="41388-918">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-918">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="41388-919">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="41388-919">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="41388-920">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="41388-920">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="41388-921">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="41388-921">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="41388-922">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="41388-922">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="41388-923">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="41388-923">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-924">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-924">AppService</span></span>

* <span data-ttu-id="41388-925">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-925">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="41388-926">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-926">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="41388-927">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-927">Batch</span></span>

* <span data-ttu-id="41388-928">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="41388-928">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="41388-929">Batch AI</span><span class="sxs-lookup"><span data-stu-id="41388-929">Batch AI</span></span>

* <span data-ttu-id="41388-930">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="41388-930">Added support for workspaces.</span></span> <span data-ttu-id="41388-931">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="41388-931">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="41388-932">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="41388-932">Added support for experiments.</span></span> <span data-ttu-id="41388-933">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="41388-933">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="41388-934">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-934">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="41388-935">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="41388-935">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="41388-936">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-936">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="41388-937">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-937">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="41388-938">[주요 변경 내용] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="41388-938">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="41388-939">[주요 변경 내용] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="41388-939">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="41388-940">[주요 변경 내용] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="41388-940">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="41388-941">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="41388-941">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="41388-942">[주요 변경 내용] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="41388-942">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="41388-943">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="41388-943">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="41388-944">[주요 변경 내용] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="41388-944">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="41388-945">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="41388-945">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="41388-946">[주요 변경 내용] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="41388-946">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="41388-947">[주요 변경 내용] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="41388-947">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="41388-948">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="41388-948">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="41388-949">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="41388-949">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="41388-950">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="41388-950">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="41388-951">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="41388-951">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="41388-952">지도</span><span class="sxs-lookup"><span data-stu-id="41388-952">Maps</span></span>

* <span data-ttu-id="41388-953">[주요 변경 내용] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-953">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="41388-954">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-954">Network</span></span>

* <span data-ttu-id="41388-955">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-955">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="41388-956">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-956">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="41388-957">#6502</span><span class="sxs-lookup"><span data-stu-id="41388-957">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="41388-958">예약</span><span class="sxs-lookup"><span data-stu-id="41388-958">Reservations</span></span>

* <span data-ttu-id="41388-959">[주요 변경 내용] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-959">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="41388-960">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-960">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="41388-961">[주요 변경 내용] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="41388-961">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="41388-962">[주요 변경 내용] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-962">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="41388-963">[주요 변경 내용] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="41388-963">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="41388-964">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-964">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="41388-965">역할</span><span class="sxs-lookup"><span data-stu-id="41388-965">Role</span></span>

* <span data-ttu-id="41388-966">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="41388-966">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="41388-967">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-967">SQL</span></span>

* <span data-ttu-id="41388-968">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="41388-968">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="41388-969">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-969">Storage</span></span>

* <span data-ttu-id="41388-970">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="41388-970">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="41388-971">VM</span><span class="sxs-lookup"><span data-stu-id="41388-971">VM</span></span>

* <span data-ttu-id="41388-972">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="41388-972">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="41388-973">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="41388-973">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="41388-974">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-974">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="41388-975">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="41388-975">June 13, 2018</span></span>

<span data-ttu-id="41388-976">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="41388-976">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="41388-977">코어</span><span class="sxs-lookup"><span data-stu-id="41388-977">Core</span></span>

* <span data-ttu-id="41388-978">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="41388-978">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="41388-979">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="41388-979">June 13, 2018</span></span>

<span data-ttu-id="41388-980">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="41388-980">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="41388-981">AKS</span><span class="sxs-lookup"><span data-stu-id="41388-981">AKS</span></span>

* <span data-ttu-id="41388-982">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-982">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="41388-983">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="41388-983">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="41388-984">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-984">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="41388-985">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-985">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="41388-986">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-986">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-987">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-987">AppService</span></span>

* <span data-ttu-id="41388-988">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-988">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="41388-989">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="41388-989">June 5, 2018</span></span>

<span data-ttu-id="41388-990">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="41388-990">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-991">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-991">Interactive</span></span>

* <span data-ttu-id="41388-992">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="41388-992">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="41388-993">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="41388-993">June 5, 2018</span></span>

<span data-ttu-id="41388-994">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="41388-994">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="41388-995">코어</span><span class="sxs-lookup"><span data-stu-id="41388-995">Core</span></span>

* <span data-ttu-id="41388-996">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-996">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="41388-997">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-997">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="41388-998">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-998">ACR</span></span>

* <span data-ttu-id="41388-999">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-999">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="41388-1000">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1000">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="41388-1001">AKS</span><span class="sxs-lookup"><span data-stu-id="41388-1001">AKS</span></span>

* <span data-ttu-id="41388-1002">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1002">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1003">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1003">Batch</span></span>

* <span data-ttu-id="41388-1004">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="41388-1004">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1005">IOT</span><span class="sxs-lookup"><span data-stu-id="41388-1005">IOT</span></span>

* <span data-ttu-id="41388-1006">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1006">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="41388-1007">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1007">Network</span></span>

* <span data-ttu-id="41388-1008">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="41388-1008">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="41388-1009">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="41388-1009">Policy Insights</span></span>

* <span data-ttu-id="41388-1010">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1010">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="41388-1011">ARM</span><span class="sxs-lookup"><span data-stu-id="41388-1011">ARM</span></span>

* <span data-ttu-id="41388-1012">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1012">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1013">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1013">SQL</span></span>

* <span data-ttu-id="41388-1014">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="41388-1014">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="41388-1015">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1015">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="41388-1016">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1016">Storage</span></span>

* <span data-ttu-id="41388-1017">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="41388-1017">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1018">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1018">VM</span></span>

* <span data-ttu-id="41388-1019">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1019">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="41388-1020">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1020">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="41388-1021">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1021">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="41388-1022">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="41388-1022">May 22, 2018</span></span>

<span data-ttu-id="41388-1023">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="41388-1023">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="41388-1024">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1024">Core</span></span>

* <span data-ttu-id="41388-1025">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1025">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1026">ACS</span></span>

* <span data-ttu-id="41388-1027">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1027">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="41388-1028">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1028">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1029">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-1029">AppService</span></span>

* <span data-ttu-id="41388-1030">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1030">Improved generic update commands</span></span>
* <span data-ttu-id="41388-1031">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1031">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="41388-1032">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1032">Container</span></span>

* <span data-ttu-id="41388-1033">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1033">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="41388-1034">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1034">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1035">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1035">Extension</span></span>

* <span data-ttu-id="41388-1036">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1036">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1037">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1037">Interactive</span></span>

* <span data-ttu-id="41388-1038">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1038">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="41388-1039">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="41388-1039">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="41388-1040">KeyVault</span></span>

* <span data-ttu-id="41388-1041">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="41388-1041">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="41388-1042">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1042">Network</span></span>

* <span data-ttu-id="41388-1043">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="41388-1043">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="41388-1044">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1044">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1045">SQL</span></span>

* <span data-ttu-id="41388-1046">[주요 변경 내용] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="41388-1046">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="41388-1047">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="41388-1047">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="41388-1048">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="41388-1048">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="41388-1049">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1049">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="41388-1050">[주요 변경 내용] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1050">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="41388-1051">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="41388-1051">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="41388-1052">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="41388-1052">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="41388-1053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="41388-1053">`edition`.</span></span> <span data-ttu-id="41388-1054">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="41388-1054">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="41388-1055">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="41388-1055">`elasticPoolName`.</span></span> <span data-ttu-id="41388-1056">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="41388-1056">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="41388-1057">[주요 변경 내용] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1057">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="41388-1058">`edition`.</span><span class="sxs-lookup"><span data-stu-id="41388-1058">`edition`.</span></span> <span data-ttu-id="41388-1059">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="41388-1059">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="41388-1060">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="41388-1060">`dtu`.</span></span> <span data-ttu-id="41388-1061">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="41388-1061">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="41388-1062">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="41388-1062">`databaseDtuMin`.</span></span> <span data-ttu-id="41388-1063">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="41388-1063">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="41388-1064">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="41388-1064">`databaseDtuMax`.</span></span> <span data-ttu-id="41388-1065">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="41388-1065">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="41388-1066">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1066">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="41388-1067">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1067">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1068">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1068">Storage</span></span>

* <span data-ttu-id="41388-1069">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1069">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="41388-1070">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1070">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1071">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1071">VM</span></span>

* <span data-ttu-id="41388-1072">[주요 변경 내용] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="41388-1072">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="41388-1073">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="41388-1073">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="41388-1074">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="41388-1074">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="41388-1075">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="41388-1075">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="41388-1076">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1076">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="41388-1077">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="41388-1077">May 7, 2018</span></span>

<span data-ttu-id="41388-1078">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="41388-1078">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="41388-1079">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1079">Core</span></span>

* <span data-ttu-id="41388-1080">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1080">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="41388-1081">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1081">Added limited support for positional arguments</span></span>
* <span data-ttu-id="41388-1082">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1082">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="41388-1083">#5591</span><span class="sxs-lookup"><span data-stu-id="41388-1083">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="41388-1084">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1084">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="41388-1085">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1085">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="41388-1086">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1086">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="41388-1087">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1087">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="41388-1088">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1088">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1089">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1089">ACR</span></span>

* <span data-ttu-id="41388-1090">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1090">Added ACR Build commands</span></span>
* <span data-ttu-id="41388-1091">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1091">Improved resource not found error messages</span></span>
* <span data-ttu-id="41388-1092">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1092">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="41388-1093">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1093">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="41388-1094">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1094">Improved repository commands error messages</span></span>
* <span data-ttu-id="41388-1095">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-1095">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1096">ACS</span></span>

* <span data-ttu-id="41388-1097">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1097">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="41388-1098">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1098">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="41388-1099">AMS</span><span class="sxs-lookup"><span data-stu-id="41388-1099">AMS</span></span>

* <span data-ttu-id="41388-1100">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="41388-1100">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1101">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1101">Appservice</span></span>

* <span data-ttu-id="41388-1102">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1102">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="41388-1103">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1103">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="41388-1104">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1104">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="41388-1105">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1105">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="41388-1106">Batch AI</span><span class="sxs-lookup"><span data-stu-id="41388-1106">Batch AI</span></span>

* <span data-ttu-id="41388-1107">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1107">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="41388-1108">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="41388-1108">Cognitive Services</span></span>

* <span data-ttu-id="41388-1109">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1109">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-1110">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-1110">Consumption</span></span>

* <span data-ttu-id="41388-1111">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1111">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="41388-1112">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1112">Container</span></span>

* <span data-ttu-id="41388-1113">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1113">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="41388-1114">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="41388-1114">Cosmos DB</span></span>

* <span data-ttu-id="41388-1115">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="41388-1115">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="41388-1116">DMS</span><span class="sxs-lookup"><span data-stu-id="41388-1116">DMS</span></span>

* <span data-ttu-id="41388-1117">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1117">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1118">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1118">Extension</span></span>

* <span data-ttu-id="41388-1119">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1119">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1120">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1120">Interactive</span></span>

* <span data-ttu-id="41388-1121">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1121">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="41388-1122">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="41388-1122">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="41388-1123">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1123">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="41388-1124">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1124">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="41388-1125">랩</span><span class="sxs-lookup"><span data-stu-id="41388-1125">Lab</span></span>

* <span data-ttu-id="41388-1126">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1126">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="41388-1127">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1127">Network</span></span>

* <span data-ttu-id="41388-1128">[주요 변경 내용] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1128">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="41388-1129">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1129">Profile</span></span>

* <span data-ttu-id="41388-1130">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1130">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="41388-1131">[주요 변경 내용] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1131">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="41388-1132">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1132">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="41388-1133">Redis</span><span class="sxs-lookup"><span data-stu-id="41388-1133">Redis</span></span>

* <span data-ttu-id="41388-1134">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1134">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="41388-1135">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1135">Deprecated `redis list-all`.</span></span> <span data-ttu-id="41388-1136">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="41388-1136">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="41388-1137">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1137">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="41388-1138">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1138">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="41388-1139">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1139">Role</span></span>

* <span data-ttu-id="41388-1140">[주요 변경 내용] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1140">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1141">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1141">Storage</span></span>

* <span data-ttu-id="41388-1142">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1142">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="41388-1143">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="41388-1143">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="41388-1144">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="41388-1144">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="41388-1145">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1145">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="41388-1146">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1146">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1147">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1147">VM</span></span>

* <span data-ttu-id="41388-1148">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1148">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="41388-1149">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1149">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="41388-1150">[주요 변경 내용] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="41388-1150">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="41388-1151">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1151">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="41388-1152">[주요 변경 내용] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1152">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="41388-1153">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1153">Added write accelerator support</span></span>
* <span data-ttu-id="41388-1154">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1154">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="41388-1155">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1155">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="41388-1156">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1156">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="41388-1157">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="41388-1157">April 10, 2018</span></span>

<span data-ttu-id="41388-1158">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="41388-1158">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1159">ACR</span></span>

* <span data-ttu-id="41388-1160">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="41388-1160">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1161">ACS</span></span>

* <span data-ttu-id="41388-1162">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1162">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1163">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1163">Appservice</span></span>

* [주요 변경 내용]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="41388-1165">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1165">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="41388-1166">BatchAI</span><span class="sxs-lookup"><span data-stu-id="41388-1166">BatchAI</span></span>

* <span data-ttu-id="41388-1167">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1167">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="41388-1168">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="41388-1168">Job level mounting</span></span>
  - <span data-ttu-id="41388-1169">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="41388-1169">Environment variables with secret values</span></span>
  - <span data-ttu-id="41388-1170">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="41388-1170">Performance counters settings</span></span>
  - <span data-ttu-id="41388-1171">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="41388-1171">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="41388-1172">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1172">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="41388-1173">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="41388-1173">Usage and limits reporting</span></span>
  - <span data-ttu-id="41388-1174">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1174">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="41388-1175">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1175">Support for custom images</span></span>
  - <span data-ttu-id="41388-1176">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1176">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="41388-1177">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1177">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="41388-1178">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1178">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="41388-1179">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-1179">National clouds are supported</span></span>
* <span data-ttu-id="41388-1180">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1180">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="41388-1181">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="41388-1181">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="41388-1182">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1182">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="41388-1183">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1183">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="41388-1184">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="41388-1184">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="41388-1185">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="41388-1185">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="41388-1186">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1186">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="41388-1187">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1187">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="41388-1188">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1188">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="41388-1189">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1189">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="41388-1190">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1190">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="41388-1191">[주요 변경 내용] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="41388-1191">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="41388-1192">[주요 변경 내용] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1192">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="41388-1193">결제</span><span class="sxs-lookup"><span data-stu-id="41388-1193">Billing</span></span>

* <span data-ttu-id="41388-1194">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1194">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-1195">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-1195">Consumption</span></span>

* <span data-ttu-id="41388-1196">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1196">Added `marketplace` commands</span></span>
* <span data-ttu-id="41388-1197">[주요 변경 내용] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1197">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="41388-1198">[주요 변경 내용] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1198">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="41388-1199">[주요 변경 내용] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1199">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="41388-1200">[주요 변경 내용] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1200">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="41388-1201">[주요 변경 내용] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1201">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="41388-1202">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1202">Container</span></span>

* <span data-ttu-id="41388-1203">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="41388-1203">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="41388-1204">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="41388-1204">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1205">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1205">Extension</span></span>

* <span data-ttu-id="41388-1206">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1206">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1207">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1207">Interactive</span></span>

* <span data-ttu-id="41388-1208">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1208">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="41388-1209">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1209">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="41388-1210">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1210">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="41388-1211">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1211">Network</span></span>

* <span data-ttu-id="41388-1212">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1212">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="41388-1213">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1213">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="41388-1214">#4910</span><span class="sxs-lookup"><span data-stu-id="41388-1214">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="41388-1215">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1215">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="41388-1216">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="41388-1216">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="41388-1217">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1217">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="41388-1218">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1218">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="41388-1219">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1219">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1220">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1220">Profile</span></span>

* <span data-ttu-id="41388-1221">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1221">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="41388-1222">[주요 변경 내용] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1222">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-1223">RDBMS</span></span>

* <span data-ttu-id="41388-1224">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1224">Added `georestore` command</span></span>
* <span data-ttu-id="41388-1225">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1225">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1226">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1226">Resource</span></span>

* <span data-ttu-id="41388-1227">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1227">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="41388-1228">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1228">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1229">SQL</span></span>

* <span data-ttu-id="41388-1230">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1230">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1231">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1231">Storage</span></span>

* <span data-ttu-id="41388-1232">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1232">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1233">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1233">VM</span></span>

* <span data-ttu-id="41388-1234">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1234">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="41388-1235">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1235">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="41388-1237">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1237">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="41388-1238">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1238">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="41388-1239">#5718</span><span class="sxs-lookup"><span data-stu-id="41388-1239">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="41388-1240">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1240">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="41388-1241">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="41388-1241">March 27, 2018</span></span>

<span data-ttu-id="41388-1242">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="41388-1242">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="41388-1243">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1243">Core</span></span>

* <span data-ttu-id="41388-1244">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="41388-1244">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1245">ACS</span></span>

* <span data-ttu-id="41388-1246">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1246">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1247">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1247">Appservice</span></span>

* <span data-ttu-id="41388-1248">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1248">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="41388-1249">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1249">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="41388-1250">Backup</span><span class="sxs-lookup"><span data-stu-id="41388-1250">Backup</span></span>

* <span data-ttu-id="41388-1251">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1251">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="41388-1252">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1252">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="41388-1253">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1253">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="41388-1254">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1254">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="41388-1255">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1255">Container</span></span>

* <span data-ttu-id="41388-1256">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1256">Added `container exec` command.</span></span> <span data-ttu-id="41388-1257">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1257">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="41388-1258">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1258">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1259">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1259">Extension</span></span>

* <span data-ttu-id="41388-1260">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1260">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="41388-1261">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1261">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="41388-1262">[주요 변경 내용] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1262">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1263">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1263">Interactive</span></span>

* <span data-ttu-id="41388-1264">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="41388-1264">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="41388-1265">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1265">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="41388-1266">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="41388-1266">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="41388-1267">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1267">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="41388-1268">랩</span><span class="sxs-lookup"><span data-stu-id="41388-1268">Lab</span></span>

* <span data-ttu-id="41388-1269">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1269">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1270">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1270">Monitor</span></span>

* <span data-ttu-id="41388-1271">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1271">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="41388-1272">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="41388-1272">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="41388-1273">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1273">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="41388-1274">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1274">Network</span></span>

* <span data-ttu-id="41388-1275">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1275">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1276">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1276">Profile</span></span>

* <span data-ttu-id="41388-1277">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1277">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-1278">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-1278">RDBMS</span></span>

* <span data-ttu-id="41388-1279">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1279">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1280">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1280">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="41388-1282">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1282">Role</span></span>

* <span data-ttu-id="41388-1283">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1283">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="41388-1284">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1284">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="41388-1285">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1285">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="41388-1286">[주요 변경 내용] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1286">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="41388-1287">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1287">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1288">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1288">Storage</span></span>

* <span data-ttu-id="41388-1289">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1289">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="41388-1290">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="41388-1290">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1291">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1291">VM</span></span>

* <span data-ttu-id="41388-1292">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1292">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="41388-1293">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1293">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="41388-1294">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1294">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="41388-1295">[주요 변경 내용] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1295">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="41388-1296">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="41388-1296">March 13, 2018</span></span>

<span data-ttu-id="41388-1297">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="41388-1297">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1298">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1298">ACR</span></span>

* <span data-ttu-id="41388-1299">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1299">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="41388-1300">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1300">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="41388-1301">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1301">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1302">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1302">ACS</span></span>

* <span data-ttu-id="41388-1303">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1303">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="41388-1304">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1304">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="41388-1305">Advisor</span><span class="sxs-lookup"><span data-stu-id="41388-1305">Advisor</span></span>

* <span data-ttu-id="41388-1306">[주요 변경 내용] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1306">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="41388-1307">[주요 변경 내용] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1307">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="41388-1308">[주요 변경 내용] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1308">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="41388-1309">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1309">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="41388-1310">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1310">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1311">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1311">Appservice</span></span>

* <span data-ttu-id="41388-1312">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1312">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="41388-1313">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1313">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="41388-1314">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="41388-1314">Eventhubs</span></span>

* <span data-ttu-id="41388-1315">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1315">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1316">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1316">Extension</span></span>

* <span data-ttu-id="41388-1317">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1317">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1318">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1318">Interactive</span></span>

* <span data-ttu-id="41388-1319">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="41388-1319">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="41388-1320">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="41388-1320">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="41388-1321">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1321">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="41388-1322">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1322">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1323">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1323">Monitor</span></span>

* <span data-ttu-id="41388-1324">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1324">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="41388-1325">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1325">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="41388-1326">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1326">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="41388-1327">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1327">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="41388-1328">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1328">Network</span></span>

* <span data-ttu-id="41388-1329">[주요 변경 내용] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1329">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="41388-1330">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="41388-1330">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="41388-1331">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1331">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="41388-1332">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1332">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1333">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1333">Profile</span></span>

* <span data-ttu-id="41388-1334">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1334">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="41388-1335">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1335">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-1336">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-1336">RDBMS</span></span>

* <span data-ttu-id="41388-1337">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1337">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="41388-1338">Service Bus</span><span class="sxs-lookup"><span data-stu-id="41388-1338">Service Bus</span></span>

* <span data-ttu-id="41388-1339">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1339">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1340">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1340">Storage</span></span>

* <span data-ttu-id="41388-1341">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1341">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="41388-1342">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1342">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1343">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1343">VM</span></span>

* <span data-ttu-id="41388-1344">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1344">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="41388-1345">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1345">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="41388-1346">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1346">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="41388-1347">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1347">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="41388-1348">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="41388-1348">February 27, 2018</span></span>

<span data-ttu-id="41388-1349">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="41388-1349">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="41388-1350">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1350">Core</span></span>

* <span data-ttu-id="41388-1351">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="41388-1351">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="41388-1352">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1352">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="41388-1353">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1353">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1354">ACS</span></span>

* <span data-ttu-id="41388-1355">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1355">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="41388-1356">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="41388-1356">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="41388-1357">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1357">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="41388-1358">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="41388-1358">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1359">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1359">Appservice</span></span>

* <span data-ttu-id="41388-1360">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="41388-1360">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="41388-1361">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1361">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="41388-1362">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="41388-1362">Cognitive Services</span></span>

* <span data-ttu-id="41388-1363">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-1363">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-1364">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-1364">Consumption</span></span>

* <span data-ttu-id="41388-1365">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1365">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="41388-1366">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-1366">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="41388-1367">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1367">Container</span></span>

* <span data-ttu-id="41388-1368">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1368">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="41388-1369">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1369">Network</span></span>

* <span data-ttu-id="41388-1370">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="41388-1370">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1371">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1371">Resource</span></span>

* <span data-ttu-id="41388-1372">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1372">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="41388-1373">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1373">Role</span></span>

* <span data-ttu-id="41388-1374">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1374">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1375">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1375">SQL</span></span>

* <span data-ttu-id="41388-1376">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1376">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1377">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1377">Storage</span></span>

* <span data-ttu-id="41388-1378">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="41388-1378">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1379">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1379">VM</span></span>

* <span data-ttu-id="41388-1380">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1380">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="41388-1381">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="41388-1381">February 13, 2018</span></span>

<span data-ttu-id="41388-1382">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="41388-1382">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="41388-1383">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1383">Core</span></span>

* <span data-ttu-id="41388-1384">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1384">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1385">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1385">ACS</span></span>

* <span data-ttu-id="41388-1386">[주요 변경 내용] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1386">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="41388-1387">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1387">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="41388-1388">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1388">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="41388-1389">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="41388-1389">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="41388-1390">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1390">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="41388-1391">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="41388-1391">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="41388-1392">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1392">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="41388-1393">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1393">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1394">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1394">Appservice</span></span>

* <span data-ttu-id="41388-1395">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1395">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="41388-1396">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1396">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="41388-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="41388-1397">CDN</span></span>

* <span data-ttu-id="41388-1398">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1398">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="41388-1399">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1399">Container</span></span>

* <span data-ttu-id="41388-1400">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1400">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="41388-1401">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1401">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-1402">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-1402">CosmosDB</span></span>

* <span data-ttu-id="41388-1403">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1403">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1404">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1404">Extension</span></span>

* <span data-ttu-id="41388-1405">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1405">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="41388-1406">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1406">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="41388-1407">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="41388-1407">Feedback</span></span>

* <span data-ttu-id="41388-1408">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1408">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1409">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1409">Interactive</span></span>

* <span data-ttu-id="41388-1410">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1410">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="41388-1411">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1411">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1412">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-1412">IoT</span></span>

* <span data-ttu-id="41388-1413">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1413">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="41388-1414">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1414">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="41388-1415">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1415">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="41388-1416">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1416">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1417">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1417">Monitor</span></span>

* <span data-ttu-id="41388-1418">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1418">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="41388-1419">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1419">Network</span></span>

* <span data-ttu-id="41388-1420">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1420">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="41388-1421">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1421">Profile</span></span>

* <span data-ttu-id="41388-1422">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1422">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1423">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1423">Resource</span></span>

* <span data-ttu-id="41388-1424">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1424">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="41388-1425">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1425">Role</span></span>

* <span data-ttu-id="41388-1426">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1426">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1427">SQL</span></span>

* <span data-ttu-id="41388-1428">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1428">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="41388-1429">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1429">Added `sql db rename`</span></span>
* <span data-ttu-id="41388-1430">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1430">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1431">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1431">Storage</span></span>

* <span data-ttu-id="41388-1432">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1432">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1433">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1433">VM</span></span>

* <span data-ttu-id="41388-1434">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1434">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="41388-1435">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1435">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="41388-1436">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="41388-1436">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="41388-1437">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="41388-1437">January 31, 2018</span></span>

<span data-ttu-id="41388-1438">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="41388-1438">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="41388-1439">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1439">Core</span></span>

* <span data-ttu-id="41388-1440">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1440">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="41388-1441">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="41388-1441">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="41388-1442">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1442">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="41388-1443">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="41388-1443">Use `--verbose` to see</span></span>
* <span data-ttu-id="41388-1444">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1444">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1445">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1445">ACS</span></span>

* <span data-ttu-id="41388-1446">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1446">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="41388-1447">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="41388-1447">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1448">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1448">Appservice</span></span>

* <span data-ttu-id="41388-1449">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="41388-1449">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="41388-1450">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="41388-1450">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="41388-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="41388-1451">CDN</span></span>

* <span data-ttu-id="41388-1452">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1452">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-1453">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-1453">CosmosDB</span></span>

* <span data-ttu-id="41388-1454">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1454">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1455">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1455">Interactive</span></span>

* <span data-ttu-id="41388-1456">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1456">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="41388-1457">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1457">Network</span></span>

* <span data-ttu-id="41388-1458">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1458">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="41388-1459">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1459">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="41388-1460">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1460">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="41388-1461">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1461">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="41388-1462">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1462">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="41388-1463">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="41388-1463">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="41388-1464">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1464">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="41388-1465">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1465">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="41388-1466">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1466">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="41388-1467">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="41388-1467">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1468">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1468">Profile</span></span>

* <span data-ttu-id="41388-1469">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1469">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1470">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1470">Resource</span></span>

* <span data-ttu-id="41388-1471">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1471">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1472">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1472">Storage</span></span>

* <span data-ttu-id="41388-1473">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1473">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="41388-1474">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1474">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="41388-1475">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1475">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="41388-1476">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1476">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="41388-1477">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1477">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1478">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1478">VM</span></span>

* <span data-ttu-id="41388-1479">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1479">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="41388-1480">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1480">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="41388-1481">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1481">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="41388-1482">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1482">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="41388-1483">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="41388-1483">January 17, 2018</span></span>

<span data-ttu-id="41388-1484">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="41388-1484">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1485">ACR</span></span>

* <span data-ttu-id="41388-1486">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1486">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="41388-1487">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1487">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1488">ACS</span></span>

* <span data-ttu-id="41388-1489">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1489">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="41388-1490">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1490">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1491">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1491">Appservice</span></span>

* <span data-ttu-id="41388-1492">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1492">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="41388-1493">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1493">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="41388-1494">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1494">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="41388-1495">Backup</span><span class="sxs-lookup"><span data-stu-id="41388-1495">Backup</span></span>

* <span data-ttu-id="41388-1496">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1496">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="41388-1497">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1497">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="41388-1498">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1498">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="41388-1499">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1499">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="41388-1500">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1500">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1501">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1501">Batch</span></span>

* <span data-ttu-id="41388-1502">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1502">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="41388-1503">클라우드</span><span class="sxs-lookup"><span data-stu-id="41388-1503">Cloud</span></span>

* <span data-ttu-id="41388-1504">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1504">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-1505">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-1505">Consumption</span></span>

* <span data-ttu-id="41388-1506">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1506">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="41388-1507">Event Grid</span><span class="sxs-lookup"><span data-stu-id="41388-1507">Event Grid</span></span>

* <span data-ttu-id="41388-1508">[주요 변경 내용] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="41388-1508">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="41388-1509">[주요 변경 내용] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="41388-1509">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="41388-1510">[주요 변경 내용] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1510">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="41388-1511">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="41388-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="41388-1512">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1512">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="41388-1513">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1513">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="41388-1514">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1514">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="41388-1515">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1515">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1516">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1516">Interactive</span></span>

* <span data-ttu-id="41388-1517">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1517">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="41388-1518">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1518">Fixed errors on startup</span></span>
* <span data-ttu-id="41388-1519">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1519">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1520">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-1520">IoT</span></span>

* <span data-ttu-id="41388-1521">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1521">Added support for device provisioning service</span></span>
* <span data-ttu-id="41388-1522">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1522">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="41388-1523">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1523">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1524">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1524">Monitor</span></span>

* <span data-ttu-id="41388-1525">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1525">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="41388-1526">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="41388-1526">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="41388-1527">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1527">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="41388-1528">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1528">Network</span></span>

* <span data-ttu-id="41388-1529">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1529">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="41388-1530">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1530">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1531">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1531">Profile</span></span>

* <span data-ttu-id="41388-1532">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1532">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="41388-1533">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1533">Role</span></span>

* <span data-ttu-id="41388-1534">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1534">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="41388-1535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="41388-1535">Service Fabric</span></span>

* <span data-ttu-id="41388-1536">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1536">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="41388-1537">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1537">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1538">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1538">VM</span></span>

* <span data-ttu-id="41388-1539">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1539">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="41388-1540">[주요 변경 내용] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1540">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="41388-1541">[주요 변경 내용] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1541">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="41388-1542">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1542">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="41388-1543">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1543">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="41388-1544">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1544">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="41388-1545">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1545">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="41388-1546">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1546">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="41388-1547">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="41388-1547">December 19, 2017</span></span>

<span data-ttu-id="41388-1548">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="41388-1548">Version 2.0.23</span></span>

* <span data-ttu-id="41388-1549">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1549">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="41388-1550">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1550">Container</span></span>

* <span data-ttu-id="41388-1551">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1551">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="41388-1552">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1552">Network</span></span>

* <span data-ttu-id="41388-1553">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1553">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="41388-1554">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1554">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1555">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1555">Storage</span></span>

* <span data-ttu-id="41388-1556">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1556">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1557">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1557">VM</span></span>

* <span data-ttu-id="41388-1558">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1558">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="41388-1559">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="41388-1559">December 5, 2017</span></span>

<span data-ttu-id="41388-1560">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="41388-1560">Version 2.0.22</span></span>

* <span data-ttu-id="41388-1561">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1561">Removed `az component` commands.</span></span> <span data-ttu-id="41388-1562">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="41388-1562">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="41388-1563">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1563">Core</span></span>
* <span data-ttu-id="41388-1564">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1564">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="41388-1565">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1565">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1566">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1566">ACS</span></span>

* <span data-ttu-id="41388-1567">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1567">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="41388-1568">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1568">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="41388-1569">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1569">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="41388-1570">Advisor</span><span class="sxs-lookup"><span data-stu-id="41388-1570">Advisor</span></span>

* <span data-ttu-id="41388-1571">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1571">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1572">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1572">Appservice</span></span>

* <span data-ttu-id="41388-1573">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1573">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="41388-1574">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1574">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="41388-1575">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1575">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="41388-1576">Consumption</span><span class="sxs-lookup"><span data-stu-id="41388-1576">Consumption</span></span>

* <span data-ttu-id="41388-1577">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1577">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="41388-1578">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1578">Container</span></span>

* <span data-ttu-id="41388-1579">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1579">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1580">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1580">Monitor</span></span>

* <span data-ttu-id="41388-1581">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1581">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1582">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1582">Resource</span></span>

* <span data-ttu-id="41388-1583">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1583">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="41388-1584">역할</span><span class="sxs-lookup"><span data-stu-id="41388-1584">Role</span></span>

* <span data-ttu-id="41388-1585">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1585">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="41388-1586">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1586">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="41388-1587">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="41388-1587">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1588">SQL</span></span>

* <span data-ttu-id="41388-1589">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1589">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="41388-1590">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1590">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1591">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1591">VM</span></span>

* <span data-ttu-id="41388-1592">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1592">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="41388-1593">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="41388-1593">November 14, 2017</span></span>

<span data-ttu-id="41388-1594">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="41388-1594">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1595">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1595">ACR</span></span>

* <span data-ttu-id="41388-1596">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1596">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="41388-1597">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1597">ACS</span></span>

* <span data-ttu-id="41388-1598">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1598">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="41388-1599">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="41388-1599">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="41388-1600">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1600">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="41388-1601">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1601">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="41388-1602">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1602">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1603">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1603">Appservice</span></span>

* <span data-ttu-id="41388-1604">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1604">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="41388-1605">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1605">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="41388-1606">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1606">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="41388-1607">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1607">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="41388-1608">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1608">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="41388-1609">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="41388-1609">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1610">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1610">Batch</span></span>

* <span data-ttu-id="41388-1611">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1611">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="41388-1612">Batchai</span><span class="sxs-lookup"><span data-stu-id="41388-1612">Batchai</span></span>

* <span data-ttu-id="41388-1613">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1613">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="41388-1614">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1614">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="41388-1615">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1615">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="41388-1616">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1616">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="41388-1617">클라우드</span><span class="sxs-lookup"><span data-stu-id="41388-1617">Cloud</span></span>

* <span data-ttu-id="41388-1618">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1618">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="41388-1619">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1619">Container</span></span>

* <span data-ttu-id="41388-1620">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1620">Added support to open multiple ports</span></span>
* <span data-ttu-id="41388-1621">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1621">Added container group restart policy</span></span>
* <span data-ttu-id="41388-1622">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1622">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="41388-1623">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="41388-1623">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="41388-1624">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="41388-1624">Data Lake Analytics</span></span>

* <span data-ttu-id="41388-1625">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1625">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="41388-1626">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="41388-1626">Data Lake Store</span></span>

* <span data-ttu-id="41388-1627">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1627">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1628">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1628">Extension</span></span>

* <span data-ttu-id="41388-1629">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1629">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="41388-1630">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1630">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1631">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-1631">IoT</span></span>

* <span data-ttu-id="41388-1632">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1632">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1633">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1633">Monitor</span></span>

* <span data-ttu-id="41388-1634">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1634">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="41388-1635">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1635">Network</span></span>

* <span data-ttu-id="41388-1636">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1636">Added support for CAA DNS records</span></span>
* <span data-ttu-id="41388-1637">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1637">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="41388-1638">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1638">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="41388-1639">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1639">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="41388-1640">예약</span><span class="sxs-lookup"><span data-stu-id="41388-1640">Reservations</span></span>

* <span data-ttu-id="41388-1641">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1641">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1642">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1642">Resource</span></span>

* <span data-ttu-id="41388-1643">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1643">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1644">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1644">SQL</span></span>

* <span data-ttu-id="41388-1645">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1645">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1646">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1646">Storage</span></span>

* <span data-ttu-id="41388-1647">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1647">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="41388-1648">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1648">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="41388-1649">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1649">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="41388-1650">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="41388-1650">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="41388-1651">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1651">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="41388-1652">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1652">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="41388-1653">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1653">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1654">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1654">VM</span></span>

* <span data-ttu-id="41388-1655">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1655">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="41388-1656">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1656">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="41388-1657">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1657">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="41388-1658">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1658">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="41388-1659">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1659">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="41388-1660">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="41388-1660">October 24, 2017</span></span>

<span data-ttu-id="41388-1661">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="41388-1661">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="41388-1662">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1662">Core</span></span>

* <span data-ttu-id="41388-1663">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="41388-1663">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1664">ACR</span></span>

* <span data-ttu-id="41388-1665">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="41388-1665">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="41388-1666">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1666">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="41388-1667">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="41388-1667">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1668">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1668">ACS</span></span>

* <span data-ttu-id="41388-1669">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1669">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="41388-1670">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1670">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1671">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1671">Appservice</span></span>

* <span data-ttu-id="41388-1672">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1672">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="41388-1673">구성 요소</span><span class="sxs-lookup"><span data-stu-id="41388-1673">Component</span></span>

* <span data-ttu-id="41388-1674">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1674">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1675">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1675">Monitor</span></span>

* <span data-ttu-id="41388-1676">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1676">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1677">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1677">Resource</span></span>

* <span data-ttu-id="41388-1678">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1678">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="41388-1679">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="41388-1679">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1680">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1680">VM</span></span>

* <span data-ttu-id="41388-1681">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1681">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="41388-1682">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="41388-1682">October 9, 2017</span></span>

<span data-ttu-id="41388-1683">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="41388-1683">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="41388-1684">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1684">Core</span></span>

* <span data-ttu-id="41388-1685">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1685">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1686">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1686">Appservice</span></span>

* <span data-ttu-id="41388-1687">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1687">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1688">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1688">Batch</span></span>

* <span data-ttu-id="41388-1689">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1689">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="41388-1690">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1690">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="41388-1691">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1691">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="41388-1692">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1692">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="41388-1693">Batchai</span><span class="sxs-lookup"><span data-stu-id="41388-1693">Batchai</span></span>

* <span data-ttu-id="41388-1694">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1694">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="41388-1695">Keyvault</span></span>

* <span data-ttu-id="41388-1696">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1696">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="41388-1697">(#4448)</span><span class="sxs-lookup"><span data-stu-id="41388-1697">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="41388-1698">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1698">Network</span></span>

* <span data-ttu-id="41388-1699">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1699">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="41388-1700">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1700">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1701">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1701">Resource</span></span>

* <span data-ttu-id="41388-1702">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1702">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="41388-1703">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1703">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="41388-1704">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1704">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="41388-1705">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1705">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1706">Sql</span><span class="sxs-lookup"><span data-stu-id="41388-1706">Sql</span></span>

* <span data-ttu-id="41388-1707">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1707">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="41388-1708">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1708">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="41388-1709">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1709">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1710">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1710">Storage</span></span>

* <span data-ttu-id="41388-1711">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1711">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1712">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1712">Vm</span></span>

* <span data-ttu-id="41388-1713">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1713">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="41388-1714">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1714">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="41388-1715">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1715">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="41388-1716">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1716">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="41388-1717">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1717">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="41388-1718">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="41388-1718">September 22, 2017</span></span>

<span data-ttu-id="41388-1719">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="41388-1719">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1720">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1720">Resource</span></span>

* <span data-ttu-id="41388-1721">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1721">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="41388-1722">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1722">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="41388-1723">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1723">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="41388-1724">[주요 변경 내용] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1724">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="41388-1725">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1725">Network</span></span>

* <span data-ttu-id="41388-1726">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1726">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="41388-1727">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1727">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="41388-1728">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1728">Added `asg` application security group commands</span></span>
* <span data-ttu-id="41388-1729">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1729">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="41388-1730">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1730">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="41388-1731">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1731">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="41388-1732">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1732">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1733">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1733">Storage</span></span>

* <span data-ttu-id="41388-1734">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1734">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="41388-1735">Event Grid</span><span class="sxs-lookup"><span data-stu-id="41388-1735">Eventgrid</span></span>

* <span data-ttu-id="41388-1736">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="41388-1736">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1737">SQL</span></span>

* <span data-ttu-id="41388-1738">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1738">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="41388-1739">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="41388-1739">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="41388-1740">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1740">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-1741">Keyvault</span><span class="sxs-lookup"><span data-stu-id="41388-1741">Keyvault</span></span>

* <span data-ttu-id="41388-1742">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1742">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1743">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1743">VM</span></span>

* <span data-ttu-id="41388-1744">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1744">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="41388-1745">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="41388-1745">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="41388-1746">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1746">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="41388-1747">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1747">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="41388-1748">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1748">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="41388-1749">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1749">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1750">ACS</span></span>

* <span data-ttu-id="41388-1751">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1751">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1752">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1752">Appservice</span></span>

* <span data-ttu-id="41388-1753">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="41388-1753">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="41388-1754">Backup</span><span class="sxs-lookup"><span data-stu-id="41388-1754">Backup</span></span>

* <span data-ttu-id="41388-1755">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1755">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="41388-1756">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="41388-1756">September 11, 2017</span></span>

<span data-ttu-id="41388-1757">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="41388-1757">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="41388-1758">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1758">Core</span></span>

* <span data-ttu-id="41388-1759">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1759">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="41388-1760">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1760">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1761">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1761">Acs</span></span>

* <span data-ttu-id="41388-1762">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1762">Added `acs list-locations` command</span></span>
* <span data-ttu-id="41388-1763">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="41388-1763">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1764">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1764">Appservice</span></span>

* <span data-ttu-id="41388-1765">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1765">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="41388-1766">CDN</span><span class="sxs-lookup"><span data-stu-id="41388-1766">CDN</span></span>

* <span data-ttu-id="41388-1767">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1767">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="41388-1768">내선 번호</span><span class="sxs-lookup"><span data-stu-id="41388-1768">Extension</span></span>

* <span data-ttu-id="41388-1769">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1769">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-1770">Keyvault</span><span class="sxs-lookup"><span data-stu-id="41388-1770">Keyvault</span></span>

* <span data-ttu-id="41388-1771">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1771">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="41388-1772">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1772">Network</span></span>

* <span data-ttu-id="41388-1773">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1773">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="41388-1774">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-1774">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="41388-1775">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1775">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="41388-1776">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1776">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="41388-1777">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1777">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="41388-1778">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-1778">Resource</span></span>

* <span data-ttu-id="41388-1779">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1779">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="41388-1780">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1780">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="41388-1781">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="41388-1781">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="41388-1782">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="41388-1782">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="41388-1783">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-1783">SQL</span></span>

* <span data-ttu-id="41388-1784">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1784">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1785">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1785">VM</span></span>

* <span data-ttu-id="41388-1786">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1786">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="41388-1787">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="41388-1787">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="41388-1788">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1788">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="41388-1789">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1789">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="41388-1790">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1790">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="41388-1791">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="41388-1791">August 31, 2017</span></span>

<span data-ttu-id="41388-1792">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="41388-1792">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-1793">Keyvault</span><span class="sxs-lookup"><span data-stu-id="41388-1793">Keyvault</span></span>

* <span data-ttu-id="41388-1794">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1794">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="41388-1795">Sf</span><span class="sxs-lookup"><span data-stu-id="41388-1795">Sf</span></span>

* <span data-ttu-id="41388-1796">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1796">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1797">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1797">Storage</span></span>

* <span data-ttu-id="41388-1798">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1798">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="41388-1799">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="41388-1799">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="41388-1800">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="41388-1800">August 28, 2017</span></span>

<span data-ttu-id="41388-1801">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="41388-1801">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="41388-1802">CLI</span><span class="sxs-lookup"><span data-stu-id="41388-1802">CLI</span></span>

* <span data-ttu-id="41388-1803">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1803">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1804">ACS</span></span>

* <span data-ttu-id="41388-1805">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1805">Corrected preview regions</span></span>
* <span data-ttu-id="41388-1806">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1806">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="41388-1807">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="41388-1807">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1808">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1808">Appservice</span></span>

* <span data-ttu-id="41388-1809">[주요 변경 내용] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1809">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="41388-1810">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1810">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="41388-1811">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1811">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="41388-1812">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1812">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="41388-1813">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="41388-1813">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1814">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-1814">IoT</span></span>

* <span data-ttu-id="41388-1815">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1815">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="41388-1816">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1816">Network</span></span>

* <span data-ttu-id="41388-1817">[주요 변경 내용] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1817">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="41388-1818">[주요 변경 내용] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1818">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="41388-1819">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1819">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="41388-1820">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1820">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="41388-1821">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1821">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1822">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1822">Profile</span></span>

* <span data-ttu-id="41388-1823">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1823">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="41388-1824">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="41388-1824">Service Fabric</span></span>

* <span data-ttu-id="41388-1825">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1825">Preview release</span></span>
* <span data-ttu-id="41388-1826">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="41388-1826">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="41388-1827">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1827">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="41388-1828">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1828">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1829">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1829">Storage</span></span>

* <span data-ttu-id="41388-1830">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1830">Enabled setting blob tier</span></span>
* <span data-ttu-id="41388-1831">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1831">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="41388-1832">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1832">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="41388-1833">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1833">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="41388-1834">[주요 변경 내용] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1834">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="41388-1835">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1835">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1836">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1836">VM</span></span>

* <span data-ttu-id="41388-1837">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1837">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="41388-1838">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1838">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="41388-1839">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1839">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="41388-1840">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1840">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="41388-1841">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1841">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="41388-1842">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1842">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="41388-1843">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="41388-1843">August 15, 2017</span></span>

<span data-ttu-id="41388-1844">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="41388-1844">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1845">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1845">ACS</span></span>

* <span data-ttu-id="41388-1846">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1846">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1847">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1847">Appservice</span></span>

* <span data-ttu-id="41388-1848">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1848">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="41388-1849">Event Grid</span><span class="sxs-lookup"><span data-stu-id="41388-1849">Event Grid</span></span>

* <span data-ttu-id="41388-1850">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1850">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="41388-1851">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="41388-1851">August 11, 2017</span></span>

<span data-ttu-id="41388-1852">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="41388-1852">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1853">ACS</span></span>

* <span data-ttu-id="41388-1854">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1854">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1855">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1855">Batch</span></span>

* <span data-ttu-id="41388-1856">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1856">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="41388-1857">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1857">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="41388-1858">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1858">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="41388-1859">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1859">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="41388-1860">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1860">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="41388-1861">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1861">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="41388-1862">구성 요소</span><span class="sxs-lookup"><span data-stu-id="41388-1862">Component</span></span>

* <span data-ttu-id="41388-1863">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1863">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="41388-1864">컨테이너</span><span class="sxs-lookup"><span data-stu-id="41388-1864">Container</span></span>

* <span data-ttu-id="41388-1865">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1865">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="41388-1866">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="41388-1866">Data Lake Store</span></span>

* <span data-ttu-id="41388-1867">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1867">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="41388-1868">Event Grid</span><span class="sxs-lookup"><span data-stu-id="41388-1868">Event Grid</span></span>

* <span data-ttu-id="41388-1869">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-1869">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="41388-1870">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1870">Network</span></span>

* <span data-ttu-id="41388-1871">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1871">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="41388-1872">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1872">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="41388-1873">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1873">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="41388-1874">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1874">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="41388-1875">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-1875">Profile</span></span>

* <span data-ttu-id="41388-1876">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1876">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="41388-1877">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-1877">Storage</span></span>

* <span data-ttu-id="41388-1878">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-1878">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="41388-1879">VM</span><span class="sxs-lookup"><span data-stu-id="41388-1879">VM</span></span>

* <span data-ttu-id="41388-1880">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1880">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="41388-1881">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1881">Exposed `list-skus` command</span></span>
* <span data-ttu-id="41388-1882">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1882">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="41388-1883">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1883">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="41388-1884">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1884">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="41388-1885">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="41388-1885">July 28, 2017</span></span>

<span data-ttu-id="41388-1886">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="41388-1886">Version 2.0.12</span></span>

* <span data-ttu-id="41388-1887">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1887">Added container commands</span></span>
* <span data-ttu-id="41388-1888">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1888">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="41388-1889">코어</span><span class="sxs-lookup"><span data-stu-id="41388-1889">Core</span></span>

* <span data-ttu-id="41388-1890">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="41388-1890">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="41388-1891">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="41388-1891">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="41388-1892">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="41388-1892">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="41388-1893">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="41388-1893">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="41388-1894">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="41388-1894">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="41388-1895">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="41388-1895">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="41388-1896">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="41388-1896">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="41388-1897">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="41388-1897">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="41388-1898">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="41388-1898">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="41388-1899">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="41388-1899">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="41388-1900">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="41388-1900">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="41388-1901">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="41388-1901">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="41388-1902">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1902">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="41388-1903">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1903">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="41388-1904">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1904">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="41388-1905">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="41388-1905">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="41388-1906">ACR</span><span class="sxs-lookup"><span data-stu-id="41388-1906">ACR</span></span>

* <span data-ttu-id="41388-1907">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1907">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="41388-1908">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-1908">Support SKU update for managed registries</span></span>
* <span data-ttu-id="41388-1909">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1909">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="41388-1910">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1910">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="41388-1911">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1911">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="41388-1912">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1912">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="41388-1913">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-1913">ACS</span></span>

* <span data-ttu-id="41388-1914">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="41388-1914">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-1915">App Service</span><span class="sxs-lookup"><span data-stu-id="41388-1915">Appservice</span></span>

* <span data-ttu-id="41388-1916">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1916">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="41388-1917">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1917">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="41388-1918">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1918">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="41388-1919">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="41388-1919">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="41388-1920">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="41388-1920">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="41388-1921">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="41388-1921">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="41388-1922">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="41388-1922">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="41388-1923">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="41388-1923">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="41388-1924">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1924">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="41388-1925">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1925">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="41388-1926">Batch</span><span class="sxs-lookup"><span data-stu-id="41388-1926">Batch</span></span>

* <span data-ttu-id="41388-1927">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1927">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="41388-1928">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1928">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="41388-1929">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1929">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="41388-1930">CDN</span><span class="sxs-lookup"><span data-stu-id="41388-1930">CDN</span></span>

* <span data-ttu-id="41388-1931">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="41388-1931">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="41388-1932">클라우드</span><span class="sxs-lookup"><span data-stu-id="41388-1932">Cloud</span></span>

* <span data-ttu-id="41388-1933">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1933">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="41388-1934">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-1934">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="41388-1935">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-1935">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="41388-1936">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="41388-1936">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="41388-1937">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="41388-1937">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-1938">CosmosDB</span></span>

* <span data-ttu-id="41388-1939">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1939">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="41388-1940">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1940">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="41388-1941">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="41388-1941">Data Lake Analytics</span></span>

* <span data-ttu-id="41388-1942">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1942">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="41388-1943">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1943">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="41388-1944">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1944">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="41388-1945">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="41388-1945">Data Lake Store</span></span>

* <span data-ttu-id="41388-1946">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1946">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="41388-1947">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1947">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="41388-1948">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1948">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="41388-1949">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="41388-1949">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="41388-1950">대화형</span><span class="sxs-lookup"><span data-stu-id="41388-1950">Interactive</span></span>

* <span data-ttu-id="41388-1951">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1951">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="41388-1952">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1952">Increased test coverage</span></span>
* <span data-ttu-id="41388-1953">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-1953">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="41388-1954">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="41388-1954">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="41388-1955">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="41388-1955">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="41388-1956">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="41388-1956">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="41388-1957">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="41388-1957">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="41388-1958">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1958">Added `--progress` flag</span></span>
* <span data-ttu-id="41388-1959">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-1959">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="41388-1960">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="41388-1960">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="41388-1961">IoT</span><span class="sxs-lookup"><span data-stu-id="41388-1961">IoT</span></span>

* <span data-ttu-id="41388-1962">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-1962">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="41388-1963">(#3934)</span><span class="sxs-lookup"><span data-stu-id="41388-1963">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="41388-1964">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="41388-1964">Key vault</span></span>

* <span data-ttu-id="41388-1965">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="41388-1965">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="41388-1966">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="41388-1966">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="41388-1967">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="41388-1967">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="41388-1968">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="41388-1968">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="41388-1969">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="41388-1969">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="41388-1970">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="41388-1970">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="41388-1971">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="41388-1971">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="41388-1972">(#3307)</span><span class="sxs-lookup"><span data-stu-id="41388-1972">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="41388-1973">랩</span><span class="sxs-lookup"><span data-stu-id="41388-1973">Lab</span></span>

* <span data-ttu-id="41388-1974">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1974">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="41388-1975">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1975">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-1976">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-1976">Monitor</span></span>

* <span data-ttu-id="41388-1977">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="41388-1977">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="41388-1978">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1978">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="41388-1979">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1979">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="41388-1980">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1980">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="41388-1981">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="41388-1981">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="41388-1982">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="41388-1982">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="41388-1983">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1983">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="41388-1984">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1984">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="41388-1985">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1985">`location` no longer required</span></span>
  * <span data-ttu-id="41388-1986">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1986">Add name and ID support for target</span></span>
  * <span data-ttu-id="41388-1987">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1987">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="41388-1988">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1988">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="41388-1989">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1989">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="41388-1990">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1990">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="41388-1991">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-1991">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="41388-1992">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1992">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="41388-1993">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-1993">Network</span></span>

* <span data-ttu-id="41388-1994">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1994">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="41388-1995">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1995">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="41388-1996">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1996">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="41388-1997">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1997">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="41388-1998">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-1998">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="41388-1999">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-1999">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="41388-2000">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="41388-2000">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="41388-2001">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="41388-2001">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="41388-2002">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="41388-2002">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="41388-2003">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="41388-2003">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="41388-2004">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="41388-2004">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="41388-2005">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="41388-2005">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="41388-2006">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="41388-2006">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="41388-2007">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="41388-2007">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="41388-2008">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2008">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="41388-2009">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-2009">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="41388-2010">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2010">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="41388-2011">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2011">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="41388-2012">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2012">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="41388-2013">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2013">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="41388-2014">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2014">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="41388-2015">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2015">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="41388-2016">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-2016">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="41388-2017">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-2017">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="41388-2018">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-2018">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="41388-2019">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-2019">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="41388-2020">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="41388-2020">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="41388-2021">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-2021">Profile</span></span>

* <span data-ttu-id="41388-2022">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2022">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="41388-2023">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2023">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="41388-2024">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="41388-2024">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="41388-2025">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2025">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="41388-2026">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2026">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="41388-2027">RDBMS</span><span class="sxs-lookup"><span data-stu-id="41388-2027">RDBMS</span></span>

* <span data-ttu-id="41388-2028">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="41388-2028">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="41388-2029">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="41388-2029">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="41388-2030">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="41388-2030">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="41388-2031">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="41388-2031">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="41388-2032">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-2032">Resource</span></span>

* <span data-ttu-id="41388-2033">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-2033">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="41388-2034">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="41388-2034">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="41388-2035">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2035">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="41388-2036">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2036">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="41388-2037">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="41388-2037">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="41388-2038">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2038">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="41388-2039">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="41388-2039">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="41388-2040">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2040">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="41388-2041">역할</span><span class="sxs-lookup"><span data-stu-id="41388-2041">Role</span></span>

* <span data-ttu-id="41388-2042">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2042">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="41388-2043">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="41388-2043">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="41388-2044">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="41388-2044">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="41388-2045">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="41388-2045">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="41388-2046">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2046">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="41388-2047">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="41388-2047">Service Fabric</span></span>
* <span data-ttu-id="41388-2048">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="41388-2048">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="41388-2049">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="41388-2049">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="41388-2050">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="41388-2050">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="41388-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-2051">SQL</span></span>

* <span data-ttu-id="41388-2052">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-2052">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="41388-2053">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="41388-2053">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="41388-2054">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2054">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="41388-2055">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-2055">Storage</span></span>

* <span data-ttu-id="41388-2056">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="41388-2056">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="41388-2057">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="41388-2057">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="41388-2058">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="41388-2058">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="41388-2059">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-2059">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="41388-2060">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="41388-2060">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="41388-2061">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="41388-2061">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="41388-2062">VM</span><span class="sxs-lookup"><span data-stu-id="41388-2062">VM</span></span>

* <span data-ttu-id="41388-2063">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2063">Support configuring nsg</span></span>
* <span data-ttu-id="41388-2064">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2064">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="41388-2065">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="41388-2065">Support managed service identities</span></span>
* <span data-ttu-id="41388-2066">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="41388-2066">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="41388-2067">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="41388-2067">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="41388-2068">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="41388-2068">May 10, 2017</span></span>

<span data-ttu-id="41388-2069">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="41388-2069">Version 2.0.6</span></span>

* <span data-ttu-id="41388-2070">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="41388-2070">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="41388-2071">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2071">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="41388-2072">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="41388-2072">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="41388-2073">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="41388-2073">Include Cognitive Services module</span></span>
* <span data-ttu-id="41388-2074">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="41388-2074">Include Service Fabric module</span></span>
* <span data-ttu-id="41388-2075">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="41388-2075">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="41388-2076">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2076">Add support for CDN commands</span></span>
* <span data-ttu-id="41388-2077">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="41388-2077">Remove Container module</span></span>
* <span data-ttu-id="41388-2078">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="41388-2078">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="41388-2079">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="41388-2079">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="41388-2080">코어</span><span class="sxs-lookup"><span data-stu-id="41388-2080">Core</span></span>

* <span data-ttu-id="41388-2081">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="41388-2081">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="41388-2082">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="41388-2082">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="41388-2083">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="41388-2083">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="41388-2084">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="41388-2084">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="41388-2085">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="41388-2085">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="41388-2086">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="41388-2086">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="41388-2087">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="41388-2087">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="41388-2088">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="41388-2088">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="41388-2089">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="41388-2089">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="41388-2090">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="41388-2090">core: Improved performance</span></span>
* <span data-ttu-id="41388-2091">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="41388-2091">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="41388-2092">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="41388-2092">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="41388-2093">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-2093">ACS</span></span>

* <span data-ttu-id="41388-2094">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2094">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="41388-2095">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="41388-2095">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="41388-2096">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="41388-2096">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="41388-2097">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="41388-2097">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-2098">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-2098">AppService</span></span>

* <span data-ttu-id="41388-2099">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="41388-2099">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="41388-2100">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2100">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="41388-2101">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="41388-2101">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="41388-2102">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="41388-2102">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="41388-2103">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="41388-2103">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="41388-2104">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="41388-2104">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="41388-2105">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="41388-2105">support slot swap with preview</span></span>
* <span data-ttu-id="41388-2106">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="41388-2106">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="41388-2107">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="41388-2107">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="41388-2108">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="41388-2108">CosmosDB</span></span>

* <span data-ttu-id="41388-2109">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="41388-2109">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="41388-2110">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2110">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="41388-2111">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2111">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="41388-2112">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2112">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="41388-2113">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="41388-2113">Data Lake Analytics</span></span>

* <span data-ttu-id="41388-2114">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2114">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="41388-2115">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2115">Add support for new catalog item type: package.</span></span> <span data-ttu-id="41388-2116">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="41388-2116">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="41388-2117">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="41388-2117">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="41388-2118">테이블</span><span class="sxs-lookup"><span data-stu-id="41388-2118">Table</span></span>
  * <span data-ttu-id="41388-2119">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="41388-2119">Table valued function</span></span>
  * <span data-ttu-id="41388-2120">보기</span><span class="sxs-lookup"><span data-stu-id="41388-2120">View</span></span>
  * <span data-ttu-id="41388-2121">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="41388-2121">Table Statistics.</span></span> <span data-ttu-id="41388-2122">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="41388-2122">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="41388-2123">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="41388-2123">Data Lake Store</span></span>

* <span data-ttu-id="41388-2124">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="41388-2124">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="41388-2125">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="41388-2125">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="41388-2126">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="41388-2126">missed help for access show.</span></span> <span data-ttu-id="41388-2127">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2127">adding it.</span></span> <span data-ttu-id="41388-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="41388-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="41388-2129">찾기</span><span class="sxs-lookup"><span data-stu-id="41388-2129">Find</span></span>

* <span data-ttu-id="41388-2130">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="41388-2130">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="41388-2131">KeyVault</span><span class="sxs-lookup"><span data-stu-id="41388-2131">KeyVault</span></span>

* <span data-ttu-id="41388-2132">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2132">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="41388-2133">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="41388-2133">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="41388-2134">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2134">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="41388-2135">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2135">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="41388-2136">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="41388-2136">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="41388-2137">랩</span><span class="sxs-lookup"><span data-stu-id="41388-2137">Lab</span></span>

* <span data-ttu-id="41388-2138">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2138">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="41388-2139">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2139">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="41388-2140">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="41388-2140">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="41388-2141">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="41388-2141">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="41388-2142">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2142">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="41388-2143">모니터</span><span class="sxs-lookup"><span data-stu-id="41388-2143">Monitor</span></span>

* <span data-ttu-id="41388-2144">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="41388-2144">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="41388-2145">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="41388-2145">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="41388-2146">네트워크</span><span class="sxs-lookup"><span data-stu-id="41388-2146">Network</span></span>

* <span data-ttu-id="41388-2147">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2147">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="41388-2148">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2148">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="41388-2149">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2149">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="41388-2150">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2150">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="41388-2151">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2151">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="41388-2152">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2152">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="41388-2153">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2153">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="41388-2154">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2154">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="41388-2155">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2155">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="41388-2156">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2156">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="41388-2157">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="41388-2157">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="41388-2158">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2158">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="41388-2159">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2159">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="41388-2160">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2160">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="41388-2161">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="41388-2161">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="41388-2162">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2162">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="41388-2163">프로필</span><span class="sxs-lookup"><span data-stu-id="41388-2163">Profile</span></span>

* <span data-ttu-id="41388-2164">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="41388-2164">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="41388-2165">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="41388-2165">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="41388-2166">Redis</span><span class="sxs-lookup"><span data-stu-id="41388-2166">Redis</span></span>

* <span data-ttu-id="41388-2167">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2167">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="41388-2168">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="41388-2168">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="41388-2169">리소스</span><span class="sxs-lookup"><span data-stu-id="41388-2169">Resource</span></span>

* <span data-ttu-id="41388-2170">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="41388-2170">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="41388-2171">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="41388-2171">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="41388-2172">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="41388-2172">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="41388-2173">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2173">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="41388-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="41388-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="41388-2175">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2175">Add docs for az lock update.</span></span> <span data-ttu-id="41388-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="41388-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="41388-2177">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2177">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="41388-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="41388-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="41388-2179">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2179">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="41388-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="41388-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="41388-2181">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="41388-2181">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="41388-2182">역할</span><span class="sxs-lookup"><span data-stu-id="41388-2182">Role</span></span>

* <span data-ttu-id="41388-2183">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="41388-2183">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="41388-2184">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="41388-2184">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="41388-2185">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="41388-2185">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="41388-2186">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="41388-2186">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="41388-2187">SQL</span><span class="sxs-lookup"><span data-stu-id="41388-2187">SQL</span></span>

* <span data-ttu-id="41388-2188">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="41388-2188">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="41388-2189">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="41388-2189">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="41388-2190">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-2190">Storage</span></span>

* <span data-ttu-id="41388-2191">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="41388-2191">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="41388-2192">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2192">Add support for incremental blob copy</span></span>
* <span data-ttu-id="41388-2193">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2193">Add support for large block blob upload</span></span>
* <span data-ttu-id="41388-2194">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="41388-2194">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="41388-2195">VM</span><span class="sxs-lookup"><span data-stu-id="41388-2195">VM</span></span>

* <span data-ttu-id="41388-2196">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="41388-2196">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="41388-2197">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="41388-2197">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="41388-2198">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="41388-2198">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="41388-2199">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="41388-2199">az vm/vmss disk</span></span>
  3. <span data-ttu-id="41388-2200">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2200">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="41388-2201">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="41388-2201">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="41388-2202">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="41388-2202">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="41388-2203">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="41388-2203">April 3, 2017</span></span>

<span data-ttu-id="41388-2204">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="41388-2204">Version 2.0.2</span></span>

<span data-ttu-id="41388-2205">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2205">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="41388-2206">코어</span><span class="sxs-lookup"><span data-stu-id="41388-2206">Core</span></span>

* <span data-ttu-id="41388-2207">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="41388-2207">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="41388-2208">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="41388-2208">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="41388-2209">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="41388-2209">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="41388-2210">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="41388-2210">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="41388-2211">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="41388-2211">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="41388-2212">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="41388-2212">Add prompting for missing template parameters.</span></span> <span data-ttu-id="41388-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="41388-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="41388-2214">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="41388-2214">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="41388-2215">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="41388-2215">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="41388-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="41388-2216">ACS</span></span>

* <span data-ttu-id="41388-2217">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="41388-2217">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="41388-2218">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="41388-2218">Add support for ssh key password prompting.</span></span> <span data-ttu-id="41388-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="41388-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="41388-2220">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="41388-2220">Add support for windows clusters.</span></span> <span data-ttu-id="41388-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="41388-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="41388-2222">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="41388-2222">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="41388-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="41388-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="41388-2224">AppService</span><span class="sxs-lookup"><span data-stu-id="41388-2224">AppService</span></span>

* <span data-ttu-id="41388-2225">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="41388-2225">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="41388-2226">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="41388-2226">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="41388-2227">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="41388-2227">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="41388-2228">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="41388-2228">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="41388-2229">DataLake</span><span class="sxs-lookup"><span data-stu-id="41388-2229">DataLake</span></span>

* <span data-ttu-id="41388-2230">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-2230">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="41388-2231">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="41388-2231">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="41388-2232">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="41388-2232">DocuemntDB</span></span>

* <span data-ttu-id="41388-2233">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="41388-2233">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="41388-2234">VM</span><span class="sxs-lookup"><span data-stu-id="41388-2234">VM</span></span>

* <span data-ttu-id="41388-2235">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="41388-2235">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="41388-2236">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="41388-2236">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="41388-2237">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="41388-2237">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="41388-2238">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="41388-2238">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="41388-2239">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="41388-2239">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="41388-2240">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="41388-2240">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="41388-2241">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="41388-2241">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="41388-2242">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="41388-2242">February 27, 2017</span></span>

<span data-ttu-id="41388-2243">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="41388-2243">Version 2.0.0</span></span>

<span data-ttu-id="41388-2244">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2244">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="41388-2245">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="41388-2245">Container Service (acs)</span></span>
- <span data-ttu-id="41388-2246">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="41388-2246">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="41388-2247">네트워킹</span><span class="sxs-lookup"><span data-stu-id="41388-2247">Networking</span></span>
- <span data-ttu-id="41388-2248">Storage</span><span class="sxs-lookup"><span data-stu-id="41388-2248">Storage</span></span>

<span data-ttu-id="41388-2249">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2249">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="41388-2250">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2250">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="41388-2251">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2251">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="41388-2252">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2252">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="41388-2253">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="41388-2253">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="41388-2254">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41388-2254">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="41388-2255">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="41388-2255">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="41388-2256">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="41388-2256">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="41388-2257">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="41388-2257">Provide feedback from the command line with the `az feedback` command</span></span>


---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/18/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8431946b169b550bfd3f5120cf26e2feeb5c9f2c
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194854"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="11308-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="11308-103">Azure CLI release notes</span></span>

## <a name="june-18-2019"></a><span data-ttu-id="11308-104">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="11308-104">June 18, 2019</span></span>

<span data-ttu-id="11308-105">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="11308-105">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="11308-106">코어</span><span class="sxs-lookup"><span data-stu-id="11308-106">Core</span></span>

<span data-ttu-id="11308-107">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-107">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="11308-108">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-108">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="11308-109">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-109">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="11308-110">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-110">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="11308-111">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-111">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="11308-112">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-112">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="11308-113">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-113">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="11308-114">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-114">ACR</span></span>
* <span data-ttu-id="11308-115">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-115">Added 'acr check-health' command</span></span>
* <span data-ttu-id="11308-116">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="11308-116">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="11308-117">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-117">ACS</span></span>
* <span data-ttu-id="11308-118">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="11308-118">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="11308-119">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-119">AMS</span></span>
* <span data-ttu-id="11308-120">[호환성이 손상되는 변경] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-120">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-121">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-121">AppService</span></span>
* <span data-ttu-id="11308-122">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="11308-122">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="11308-123">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-123">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="11308-124">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-124">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="11308-125">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-125">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="11308-126">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-126">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="11308-127">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-127">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="11308-128">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-128">Batch</span></span>
* <span data-ttu-id="11308-129">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-129">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-130">BatchAI</span><span class="sxs-lookup"><span data-stu-id="11308-130">BatchAI</span></span>
* <span data-ttu-id="11308-131">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="11308-131">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-132">BotService</span><span class="sxs-lookup"><span data-stu-id="11308-132">BotService</span></span>
* <span data-ttu-id="11308-133">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="11308-133">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-134">CosmosDB</span></span>
* <span data-ttu-id="11308-135">[사용 되지 않음] `cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-135">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="11308-136">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="11308-136">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="11308-137">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-137">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="11308-138">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-138">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="11308-139">EventGrid</span><span class="sxs-lookup"><span data-stu-id="11308-139">EventGrid</span></span>
* <span data-ttu-id="11308-140">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-140">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="11308-141">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-141">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="11308-142">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-142">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="11308-143">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="11308-143">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="11308-144">[호환성이 손상되는 변경] `eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="11308-144">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="11308-145">HDInsight</span><span class="sxs-lookup"><span data-stu-id="11308-145">HDInsight</span></span>
* <span data-ttu-id="11308-146">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-146">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="11308-147">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-147">IoT</span></span>
* <span data-ttu-id="11308-148">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-148">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="11308-149">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-149">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="11308-150">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-150">Network</span></span>
* <span data-ttu-id="11308-151">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-151">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="11308-152">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-152">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="11308-153">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-153">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="11308-154">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-154">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="11308-155">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-155">Resource</span></span>
* <span data-ttu-id="11308-156">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-156">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="11308-157">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="11308-157">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="11308-158">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11308-158">ServiceBus</span></span>
* <span data-ttu-id="11308-159">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-159">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="11308-160">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-160">SQL</span></span>
* <span data-ttu-id="11308-161">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-161">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="11308-162">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-162">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="11308-163">SQLVm</span><span class="sxs-lookup"><span data-stu-id="11308-163">SQLVm</span></span>
* <span data-ttu-id="11308-164">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-164">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="11308-165">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-165">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="11308-166">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-166">Storage</span></span>
* <span data-ttu-id="11308-167">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-167">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="11308-168">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="11308-168">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="11308-169">VM</span><span class="sxs-lookup"><span data-stu-id="11308-169">VM</span></span>
* <span data-ttu-id="11308-170">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-170">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="11308-171">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="11308-171">June 4, 2019</span></span>

<span data-ttu-id="11308-172">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="11308-172">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="11308-173">코어</span><span class="sxs-lookup"><span data-stu-id="11308-173">Core</span></span>
* <span data-ttu-id="11308-174">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-174">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="11308-175">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-175">ACR</span></span>
* <span data-ttu-id="11308-176">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-176">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="11308-177">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-177">ACS</span></span>
* <span data-ttu-id="11308-178">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="11308-178">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="11308-179">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="11308-179">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="11308-180">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-180">Batch</span></span>
* <span data-ttu-id="11308-181">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-181">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="11308-182">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-182">IoT</span></span>
* <span data-ttu-id="11308-183">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-183">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="11308-184">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-184">Network</span></span>
* <span data-ttu-id="11308-185">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-185">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="11308-186">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-186">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="11308-187">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-187">Resource</span></span>
* <span data-ttu-id="11308-188">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-188">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="11308-189">역할</span><span class="sxs-lookup"><span data-stu-id="11308-189">Role</span></span>
* <span data-ttu-id="11308-190">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-190">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="11308-191">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="11308-191">Compute</span></span>
* <span data-ttu-id="11308-192">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-192">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="11308-193">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="11308-193">May 21, 2019</span></span>

<span data-ttu-id="11308-194">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="11308-194">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="11308-195">코어</span><span class="sxs-lookup"><span data-stu-id="11308-195">Core</span></span>
* <span data-ttu-id="11308-196">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-196">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="11308-197">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-197">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="11308-198">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-198">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="11308-199">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-199">ACR</span></span>
* <span data-ttu-id="11308-200">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-200">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="11308-201">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-201">ACS</span></span>
* <span data-ttu-id="11308-202">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-202">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-203">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-203">AppService</span></span>
* <span data-ttu-id="11308-204">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-204">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="11308-205">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-205">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="11308-206">[호환성이 손상되는 변경] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-206">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="11308-207">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-207">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="11308-208">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-208">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="11308-209">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-209">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="11308-210">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-210">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-211">BotService</span><span class="sxs-lookup"><span data-stu-id="11308-211">BotService</span></span>
* <span data-ttu-id="11308-212">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-212">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="11308-213">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-213">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-214">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-214">Consumption</span></span>
* <span data-ttu-id="11308-215">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-215">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="11308-216">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-216">IoT</span></span>
* <span data-ttu-id="11308-217">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-217">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="11308-218">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-218">Network</span></span>
* [호환성이 손상되는 변경]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="11308-220">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-220">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="11308-221">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-221">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-222">RDBMS</span></span>
* <span data-ttu-id="11308-223">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-223">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="11308-224">RBAC</span><span class="sxs-lookup"><span data-stu-id="11308-224">RBAC</span></span>
* <span data-ttu-id="11308-225">`role assignment`에 관리 그룹 범위가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-225">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-226">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-226">Storage</span></span>
* <span data-ttu-id="11308-227">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-227">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="11308-228">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="11308-228">Compute</span></span>
* <span data-ttu-id="11308-229">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-229">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="11308-230">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-230">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="11308-231">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="11308-231">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="11308-232">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-232">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="11308-233">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="11308-233">May 6, 2019</span></span>

<span data-ttu-id="11308-234">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="11308-234">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="11308-235">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-235">ACS</span></span>
* <span data-ttu-id="11308-236">[호환성이 손상되는 변경] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-236">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="11308-237">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-237">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="11308-238">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-238">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="11308-239">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-239">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-240">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-240">Appservice</span></span>
* <span data-ttu-id="11308-241">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-241">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="11308-242">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-242">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="11308-243">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-243">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="11308-244">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-244">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="11308-245">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-245">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="11308-246">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-246">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="11308-247">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-247">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="11308-248">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-248">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="11308-249">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-249">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="11308-250">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-250">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="11308-251">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-251">Batch</span></span>
* <span data-ttu-id="11308-252">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-252">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-253">Botservice</span><span class="sxs-lookup"><span data-stu-id="11308-253">Botservice</span></span>
* <span data-ttu-id="11308-254">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="11308-254">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="11308-255">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-255">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="11308-256">[호환성이 손상되는 변경] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-256">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="11308-257">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="11308-257">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="11308-258">[호환성이 손상되는 변경] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-258">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="11308-259">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="11308-259">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="11308-260">[호환성이 손상되는 변경] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-260">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="11308-261">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-261">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="11308-262">[호환성이 손상되는 변경] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-262">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="11308-263">[호환성이 손상되는 변경] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-263">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="11308-264">[호환성이 손상되는 변경] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-264">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="11308-265">[호환성이 손상되는 변경] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-265">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="11308-266">[호환성이 손상되는 변경] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-266">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="11308-267">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="11308-267">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="11308-268">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="11308-268">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="11308-269">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-269">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="11308-270">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-270">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="11308-271">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-271">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="11308-272">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-272">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="11308-273">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-273">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="11308-274">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-274">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="11308-275">구성</span><span class="sxs-lookup"><span data-stu-id="11308-275">Configure</span></span>
* <span data-ttu-id="11308-276">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-276">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="11308-277">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="11308-277">Eventhubs</span></span>
* <span data-ttu-id="11308-278">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-278">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="11308-279">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-279">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="11308-280">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-280">Network</span></span>
* <span data-ttu-id="11308-281">[호환성이 손상되는 변경] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="11308-281">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="11308-282">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="11308-282">Policy Insights</span></span>
* <span data-ttu-id="11308-283">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-283">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="11308-284">역할</span><span class="sxs-lookup"><span data-stu-id="11308-284">Role</span></span>
* <span data-ttu-id="11308-285">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-285">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="11308-286">Service Bus</span><span class="sxs-lookup"><span data-stu-id="11308-286">Service Bus</span></span>
* <span data-ttu-id="11308-287">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-287">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="11308-288">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-288">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="11308-289">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-289">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="11308-290">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-290">SQL</span></span>
* <span data-ttu-id="11308-291">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-291">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="11308-292">VM</span><span class="sxs-lookup"><span data-stu-id="11308-292">VM</span></span>
* <span data-ttu-id="11308-293">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-293">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="11308-294">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-294">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="11308-295">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-295">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="11308-296">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-296">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="11308-297">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-297">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="11308-298">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-298">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="11308-299">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="11308-299">April 23, 2019</span></span>

<span data-ttu-id="11308-300">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="11308-300">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="11308-301">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-301">ACS</span></span>
* <span data-ttu-id="11308-302">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-302">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="11308-303">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="11308-303">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="11308-304">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-304">AMS</span></span>
* <span data-ttu-id="11308-305">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-305">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-306">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-306">AppService</span></span>
* <span data-ttu-id="11308-307">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-307">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="11308-308">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-308">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="11308-309">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-309">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="11308-310">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-310">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="11308-311">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-311">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="11308-312">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="11308-312">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="11308-313">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-313">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="11308-314">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="11308-314">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="11308-315">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-315">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="11308-316">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="11308-316">Deployment Manager</span></span>
* <span data-ttu-id="11308-317">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="11308-317">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="11308-318">랩</span><span class="sxs-lookup"><span data-stu-id="11308-318">Lab</span></span>
* <span data-ttu-id="11308-319">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-319">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="11308-320">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-320">Network</span></span>
* <span data-ttu-id="11308-321">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-321">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="11308-322">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-322">Resource</span></span>
* <span data-ttu-id="11308-323">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="11308-323">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="11308-324">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="11308-324">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="11308-325">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-325">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="11308-326">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-326">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="11308-327">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-327">SQL</span></span>
* <span data-ttu-id="11308-328">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-328">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="11308-329">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-329">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="11308-330">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-330">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="11308-331">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-331">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-332">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-332">Storage</span></span>
* <span data-ttu-id="11308-333">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-333">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-334">VM</span><span class="sxs-lookup"><span data-stu-id="11308-334">VM</span></span>
* <span data-ttu-id="11308-335">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-335">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="11308-336">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-336">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="11308-337">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-337">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="11308-338">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="11308-338">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="11308-339">코어</span><span class="sxs-lookup"><span data-stu-id="11308-339">Core</span></span>
* <span data-ttu-id="11308-340">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-340">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="11308-341">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-341">ACR</span></span>
* <span data-ttu-id="11308-342">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-342">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="11308-343">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-343">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="11308-346">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-346">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="11308-347">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-347">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-348">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-348">AppService</span></span>
* <span data-ttu-id="11308-349">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-349">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="11308-350">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-350">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="11308-351">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="11308-351">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="11308-352">[호환성이 손상되는 변경] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="11308-352">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="11308-353">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-353">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="11308-354">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-354">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="11308-355">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-355">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-356">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-356">CDN</span></span>
* <span data-ttu-id="11308-357">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-357">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="11308-358">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="11308-358">Feedback</span></span>
* <span data-ttu-id="11308-359">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-359">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="11308-360">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-360">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="11308-361">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-361">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-362">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-362">Monitor</span></span>
* <span data-ttu-id="11308-363">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-363">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="11308-364">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-364">Network</span></span>
* <span data-ttu-id="11308-365">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-365">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="11308-366">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-366">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="11308-367">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-367">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="11308-368">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="11308-368">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="11308-369">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="11308-369">PrivateDNS</span></span>
* <span data-ttu-id="11308-370">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-370">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="11308-371">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-371">Resource</span></span>
* <span data-ttu-id="11308-372">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-372">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="11308-373">역할</span><span class="sxs-lookup"><span data-stu-id="11308-373">Role</span></span>
* <span data-ttu-id="11308-374">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-374">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="11308-375">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-375">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="11308-376">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-376">SQL</span></span>
* <span data-ttu-id="11308-377">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-377">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="11308-378">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-378">Storage</span></span>
* <span data-ttu-id="11308-379">[호환성이 손상되는 변경] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="11308-379">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="11308-380">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-380">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="11308-381">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-381">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="11308-382">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-382">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="11308-383">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="11308-383">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="11308-384">코어</span><span class="sxs-lookup"><span data-stu-id="11308-384">Core</span></span>
* <span data-ttu-id="11308-385">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-385">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="11308-386">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="11308-386">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="11308-387">클라우드</span><span class="sxs-lookup"><span data-stu-id="11308-387">Cloud</span></span>
* <span data-ttu-id="11308-388">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-388">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="11308-389">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-389">ACR</span></span>
* <span data-ttu-id="11308-390">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="11308-390">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="11308-391">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-391">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="11308-392">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-392">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="11308-393">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-393">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-394">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-394">AppService</span></span>
* <span data-ttu-id="11308-395">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-395">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="11308-396">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-396">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="11308-397">BOT Service</span><span class="sxs-lookup"><span data-stu-id="11308-397">BOT Service</span></span>
* <span data-ttu-id="11308-398">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-398">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="11308-399">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-399">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="11308-400">[호환성이 손상되는 변경] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-400">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="11308-401">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="11308-401">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-402">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-402">CDN</span></span>
* <span data-ttu-id="11308-403">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-403">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="11308-405">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-405">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="11308-406">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-406">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-407">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="11308-407">Cosmosdb</span></span>
* <span data-ttu-id="11308-408">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-408">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="11308-409">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-409">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-410">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-410">Interactive</span></span>
* <span data-ttu-id="11308-411">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-411">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-412">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-412">Monitor</span></span>
* <span data-ttu-id="11308-413">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-413">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="11308-414">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-414">Network</span></span>
* <span data-ttu-id="11308-415">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-415">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-416">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-416">Profile</span></span>
* <span data-ttu-id="11308-417">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-417">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="11308-418">Postgres</span><span class="sxs-lookup"><span data-stu-id="11308-418">Postgres</span></span> 
* <span data-ttu-id="11308-419">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-419">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="11308-420">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-420">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="11308-421">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-421">Resource</span></span>
* <span data-ttu-id="11308-422">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-422">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="11308-423">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-423">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="11308-424">그래프</span><span class="sxs-lookup"><span data-stu-id="11308-424">Graph</span></span>
* <span data-ttu-id="11308-425">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-425">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="11308-426">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-426">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="11308-427">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-427">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="11308-428">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-428">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="11308-429">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-429">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="11308-430">저장소</span><span class="sxs-lookup"><span data-stu-id="11308-430">storage</span></span>
* <span data-ttu-id="11308-431">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-431">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="11308-432">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-432">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="11308-433">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-433">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="11308-434">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-434">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="11308-435">VM</span><span class="sxs-lookup"><span data-stu-id="11308-435">VM</span></span>
* <span data-ttu-id="11308-436">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-436">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="11308-437">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="11308-437">March 12, 2019</span></span>

<span data-ttu-id="11308-438">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="11308-438">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="11308-439">코어</span><span class="sxs-lookup"><span data-stu-id="11308-439">Core</span></span>

* <span data-ttu-id="11308-440">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="11308-440">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="11308-441">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-441">ACR</span></span>

* <span data-ttu-id="11308-442">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="11308-442">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="11308-443">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-443">ACS</span></span>

* <span data-ttu-id="11308-444">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-444">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="11308-445">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-445">AppService</span></span>

* <span data-ttu-id="11308-446">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-446">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="11308-447">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="11308-447">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="11308-448">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-448">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="11308-449">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="11308-449">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-450">Botservice</span><span class="sxs-lookup"><span data-stu-id="11308-450">Botservice</span></span>

* <span data-ttu-id="11308-451">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="11308-451">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="11308-452">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-452">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="11308-453">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="11308-453">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="11308-454">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-454">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="11308-455">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-455">Container</span></span>

* <span data-ttu-id="11308-456">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-456">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="11308-457">EventHub</span><span class="sxs-lookup"><span data-stu-id="11308-457">EventHub</span></span>

* <span data-ttu-id="11308-458">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-458">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="11308-459">찾기</span><span class="sxs-lookup"><span data-stu-id="11308-459">Find</span></span>

* <span data-ttu-id="11308-460">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-460">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="11308-461">HDInsight</span><span class="sxs-lookup"><span data-stu-id="11308-461">HDInsight</span></span>

* <span data-ttu-id="11308-462">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-462">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="11308-463">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-463">Network</span></span>

* <span data-ttu-id="11308-464">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-464">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-465">Rdbms</span><span class="sxs-lookup"><span data-stu-id="11308-465">Rdbms</span></span>

* <span data-ttu-id="11308-466">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="11308-466">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="11308-467">역할</span><span class="sxs-lookup"><span data-stu-id="11308-467">Role</span></span>

* <span data-ttu-id="11308-468">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-468">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="11308-469">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-469">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="11308-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="11308-470">Service Fabric</span></span>

* <span data-ttu-id="11308-471">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-471">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="11308-472">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="11308-472">February 26, 2019</span></span>

<span data-ttu-id="11308-473">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="11308-473">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="11308-474">코어</span><span class="sxs-lookup"><span data-stu-id="11308-474">Core</span></span>

* <span data-ttu-id="11308-475">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-475">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="11308-476">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-476">ACR</span></span>

* <span data-ttu-id="11308-477">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-477">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="11308-478">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="11308-478">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="11308-479">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-479">ACS</span></span>

* <span data-ttu-id="11308-480">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-480">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-481">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-481">AppService</span></span>

* <span data-ttu-id="11308-482">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-482">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="11308-483">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-483">Batch</span></span>
* <span data-ttu-id="11308-484">[호환성이 손상되는 변경] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-484">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="11308-485">[호환성이 손상되는 변경] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-485">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="11308-486">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-486">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="11308-487">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-487">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="11308-488">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-488">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="11308-489">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-489">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-490">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-490">CosmosDB</span></span>

* <span data-ttu-id="11308-491">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-491">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="11308-492">Kusto</span><span class="sxs-lookup"><span data-stu-id="11308-492">Kusto</span></span>

* <span data-ttu-id="11308-493">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-493">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="11308-494">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-494">Network</span></span>

* <span data-ttu-id="11308-495">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-495">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="11308-496">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-496">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="11308-497">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-497">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="11308-498">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="11308-498">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="11308-499">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-499">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="11308-500">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-500">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="11308-501">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-501">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="11308-502">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-502">Resource</span></span>

* <span data-ttu-id="11308-503">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-503">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="11308-504">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-504">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="11308-505">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-505">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="11308-506">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="11308-506">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="11308-507">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-507">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="11308-508">역할</span><span class="sxs-lookup"><span data-stu-id="11308-508">Role</span></span>

* <span data-ttu-id="11308-509">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-509">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-510">VM</span><span class="sxs-lookup"><span data-stu-id="11308-510">VM</span></span>

* <span data-ttu-id="11308-511">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-511">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="11308-512">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="11308-512">February 12, 2019</span></span>

<span data-ttu-id="11308-513">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="11308-513">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="11308-514">코어</span><span class="sxs-lookup"><span data-stu-id="11308-514">Core</span></span>

* <span data-ttu-id="11308-515">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-515">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="11308-516">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-516">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="11308-517">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-517">ACR</span></span>
* <span data-ttu-id="11308-518">[호환성이 손상되는 변경] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-518">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="11308-519">[호환성이 손상되는 변경] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-519">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="11308-520">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-520">ACS</span></span>
* <span data-ttu-id="11308-521">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-521">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="11308-522">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-522">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="11308-523">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-523">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="11308-524">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-524">AMS</span></span>
* <span data-ttu-id="11308-525">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-525">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="11308-526">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-526">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-527">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-527">Appservice</span></span>
* <span data-ttu-id="11308-528">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-528">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="11308-529">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-529">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="11308-530">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-530">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="11308-531">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-531">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="11308-532">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-532">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-533">Botservice</span><span class="sxs-lookup"><span data-stu-id="11308-533">Botservice</span></span>
* <span data-ttu-id="11308-534">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-534">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="11308-535">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-535">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="11308-536">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-536">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="11308-537">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-537">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="11308-538">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-538">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="11308-539">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-539">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="11308-540">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-540">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="11308-541">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-541">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="11308-542">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="11308-542">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="11308-543">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-543">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="11308-544">Key Vault</span><span class="sxs-lookup"><span data-stu-id="11308-544">Key Vault</span></span>
* <span data-ttu-id="11308-545">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-545">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-546">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-546">Monitor</span></span>
* <span data-ttu-id="11308-547">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-547">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="11308-548">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-548">Network</span></span>
* <span data-ttu-id="11308-549">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-549">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="11308-550">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-550">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="11308-551">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-551">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="11308-552">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-552">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="11308-553">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="11308-553">Policy Insights</span></span>
* <span data-ttu-id="11308-554">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-554">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-555">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-555">RDBMS</span></span>
* <span data-ttu-id="11308-556">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-556">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="11308-557">Redis</span><span class="sxs-lookup"><span data-stu-id="11308-557">Redis</span></span>
* <span data-ttu-id="11308-558">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-558">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="11308-559">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-559">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="11308-560">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-560">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="11308-561">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-561">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="11308-562">[호환성이 손상되는 변경] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-562">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="11308-563">[호환성이 손상되는 변경] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-563">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="11308-564">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="11308-564">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="11308-565">역할</span><span class="sxs-lookup"><span data-stu-id="11308-565">Role</span></span>
* <span data-ttu-id="11308-566">[호환성이 손상되는 변경] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-566">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="11308-567">SQL VM</span><span class="sxs-lookup"><span data-stu-id="11308-567">SQL VM</span></span>
* <span data-ttu-id="11308-568">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-568">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="11308-569">VM</span><span class="sxs-lookup"><span data-stu-id="11308-569">VM</span></span>
* <span data-ttu-id="11308-570">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-570">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="11308-571">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-571">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="11308-572">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-572">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="11308-573">[호환성이 손상되는 변경] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-573">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="11308-574">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="11308-574">January 31, 2019</span></span>

<span data-ttu-id="11308-575">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="11308-575">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="11308-576">코어</span><span class="sxs-lookup"><span data-stu-id="11308-576">Core</span></span>

* <span data-ttu-id="11308-577">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="11308-577">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="11308-578">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="11308-578">January 28, 2019</span></span>

<span data-ttu-id="11308-579">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="11308-579">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="11308-580">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-580">ACR</span></span>
* <span data-ttu-id="11308-581">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-581">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="11308-582">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-582">ACS</span></span>
* <span data-ttu-id="11308-583">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="11308-583">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="11308-584">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-584">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="11308-585">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-585">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="11308-586">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-586">AMS</span></span>
* <span data-ttu-id="11308-587">[호환성이 손상되는 변경] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-587">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="11308-588">[호환성이 손상되는 변경] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-588">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-589">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-589">Appservice</span></span>
* <span data-ttu-id="11308-590">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-590">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="11308-591">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 Function Apps에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-591">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="11308-592">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-592">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="11308-593">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-593">Container</span></span>
* <span data-ttu-id="11308-594">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-594">Added `container start` command</span></span>
* <span data-ttu-id="11308-595">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-595">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="11308-596">EventGrid</span><span class="sxs-lookup"><span data-stu-id="11308-596">EventGrid</span></span>
* <span data-ttu-id="11308-597">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-597">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="11308-598">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-598">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="11308-599">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-599">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="11308-600">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-600">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="11308-601">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-601">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="11308-602">HDInsight</span><span class="sxs-lookup"><span data-stu-id="11308-602">HDInsight</span></span>
* <span data-ttu-id="11308-603">[호환성이 손상되는 변경] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-603">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="11308-604">[호환성이 손상되는 변경] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-604">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="11308-605">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-605">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="11308-606">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-606">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="11308-607">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-607">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="11308-608">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-608">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="11308-609">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-609">IoT</span></span>
* <span data-ttu-id="11308-610">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-610">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="11308-611">Kusto</span><span class="sxs-lookup"><span data-stu-id="11308-611">Kusto</span></span>
* <span data-ttu-id="11308-612">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-612">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-613">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-613">Monitor</span></span>
* <span data-ttu-id="11308-614">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-614">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="11308-615">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-615">Profile</span></span>
* <span data-ttu-id="11308-616">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-616">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="11308-617">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-617">Network</span></span>
* <span data-ttu-id="11308-618">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-618">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="11308-619">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-619">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="11308-620">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-620">Resource</span></span>
* <span data-ttu-id="11308-621">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-621">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="11308-622">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-622">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="11308-623">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="11308-623">SQL Virtual Machine</span></span>
* <span data-ttu-id="11308-624">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-624">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="11308-625">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-625">Storage</span></span>
* <span data-ttu-id="11308-626">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-626">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="11308-627">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-627">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="11308-628">VM</span><span class="sxs-lookup"><span data-stu-id="11308-628">VM</span></span>
* <span data-ttu-id="11308-629">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-629">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="11308-630">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-630">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="11308-631">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="11308-631">January 15, 2019</span></span>

<span data-ttu-id="11308-632">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="11308-632">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="11308-633">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-633">ACR</span></span>
* <span data-ttu-id="11308-634">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-634">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="11308-635">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-635">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="11308-636">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="11308-636">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="11308-637">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-637">ACS</span></span>
* <span data-ttu-id="11308-638">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-638">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-639">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-639">Appservice</span></span>
* <span data-ttu-id="11308-640">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-640">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="11308-641">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-641">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="11308-642">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-642">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="11308-643">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-643">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-644">Botservice</span><span class="sxs-lookup"><span data-stu-id="11308-644">Botservice</span></span>
* <span data-ttu-id="11308-645">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-645">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="11308-646">구성</span><span class="sxs-lookup"><span data-stu-id="11308-646">Configure</span></span>
* <span data-ttu-id="11308-647">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-647">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-648">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-648">CosmosDB</span></span>
* <span data-ttu-id="11308-649">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-649">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="11308-650">HDInsight</span><span class="sxs-lookup"><span data-stu-id="11308-650">HDInsight</span></span>
* <span data-ttu-id="11308-651">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-651">Added commands for managing applications</span></span>
* <span data-ttu-id="11308-652">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-652">Added commands for managing script actions</span></span>
* <span data-ttu-id="11308-653">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-653">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="11308-654">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-654">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="11308-655">[호환성이 손상되는 변경] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-655">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="11308-656">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-656">Network</span></span>
* <span data-ttu-id="11308-657">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-657">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="11308-658">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-658">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="11308-659">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-659">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="11308-660">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-660">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="11308-661">역할</span><span class="sxs-lookup"><span data-stu-id="11308-661">Role</span></span>
* <span data-ttu-id="11308-662">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-662">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="11308-663">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-663">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="11308-664">보안</span><span class="sxs-lookup"><span data-stu-id="11308-664">Security</span></span>
* <span data-ttu-id="11308-665">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-665">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="11308-666">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-666">Storage</span></span>
* <span data-ttu-id="11308-667">[호환성이 손상되는 변경] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-667">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="11308-668">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-668">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="11308-669">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-669">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="11308-670">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-670">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="11308-671">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-671">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="11308-672">VM</span><span class="sxs-lookup"><span data-stu-id="11308-672">VM</span></span>
* <span data-ttu-id="11308-673">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-673">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="11308-674">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-674">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="11308-675">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-675">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="11308-676">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-676">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="11308-677">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-677">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="11308-678">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-678">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="11308-679">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="11308-679">December 20, 2018</span></span>

<span data-ttu-id="11308-680">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="11308-680">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="11308-681">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-681">Appservice</span></span>
* <span data-ttu-id="11308-682">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-682">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="11308-683">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-683">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="11308-684">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-684">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="11308-685">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="11308-685">IoTCentral</span></span>
* <span data-ttu-id="11308-686">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-686">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="11308-687">역할</span><span class="sxs-lookup"><span data-stu-id="11308-687">Role</span></span>
* <span data-ttu-id="11308-688">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-688">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="11308-689">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-689">SQL</span></span>
* <span data-ttu-id="11308-690">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-690">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="11308-691">VM</span><span class="sxs-lookup"><span data-stu-id="11308-691">VM</span></span>
* <span data-ttu-id="11308-692">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-692">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="11308-693">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="11308-693">December 18, 2018</span></span>

<span data-ttu-id="11308-694">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="11308-694">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="11308-695">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-695">ACR</span></span>
* <span data-ttu-id="11308-696">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-696">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="11308-697">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="11308-697">Condensed the table layout for task list</span></span>
* <span data-ttu-id="11308-698">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-698">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="11308-699">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-699">ACS</span></span>
* <span data-ttu-id="11308-700">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="11308-700">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="11308-701">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="11308-701">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="11308-702">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-702">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="11308-703">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-703">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="11308-704">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-704">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="11308-705">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="11308-705">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-706">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-706">Appservice</span></span>
* <span data-ttu-id="11308-707">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="11308-707">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="11308-708">Botservice</span><span class="sxs-lookup"><span data-stu-id="11308-708">Botservice</span></span>
* <span data-ttu-id="11308-709">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-709">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="11308-710">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="11308-710">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="11308-711">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="11308-711">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="11308-712">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="11308-712">Reduced Kudu network calls</span></span>
* <span data-ttu-id="11308-713">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="11308-713">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-714">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-714">Consumption</span></span>
* <span data-ttu-id="11308-715">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-715">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-716">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-716">CosmosDB</span></span>
* <span data-ttu-id="11308-717">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-717">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="11308-718">지도</span><span class="sxs-lookup"><span data-stu-id="11308-718">Maps</span></span>
* <span data-ttu-id="11308-719">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-719">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="11308-720">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-720">Network</span></span>
* <span data-ttu-id="11308-721">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-721">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="11308-722">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="11308-722">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="11308-723">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-723">Resource</span></span>
* <span data-ttu-id="11308-724">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-724">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="11308-725">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-725">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-726">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-726">Storage</span></span>
*  <span data-ttu-id="11308-727">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-727">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-728">VM</span><span class="sxs-lookup"><span data-stu-id="11308-728">VM</span></span>
* <span data-ttu-id="11308-729">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-729">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="11308-730">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="11308-730">December 4, 2018</span></span>

<span data-ttu-id="11308-731">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="11308-731">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="11308-732">코어</span><span class="sxs-lookup"><span data-stu-id="11308-732">Core</span></span>
* <span data-ttu-id="11308-733">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-733">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="11308-734">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-734">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-735">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-735">Appservice</span></span>
* <span data-ttu-id="11308-736">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-736">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="11308-737">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-737">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="11308-738">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-738">Network</span></span>
* <span data-ttu-id="11308-739">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-739">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="11308-740">역할</span><span class="sxs-lookup"><span data-stu-id="11308-740">Role</span></span>
* <span data-ttu-id="11308-741">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-741">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="11308-742">VM</span><span class="sxs-lookup"><span data-stu-id="11308-742">VM</span></span>
* <span data-ttu-id="11308-743">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-743">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="11308-744">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-744">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="11308-745">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-745">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="11308-746">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-746">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="11308-747">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="11308-747">November 20, 2018</span></span>

<span data-ttu-id="11308-748">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="11308-748">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="11308-749">코어</span><span class="sxs-lookup"><span data-stu-id="11308-749">Core</span></span>
* <span data-ttu-id="11308-750">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="11308-750">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="11308-751">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-751">ACR</span></span>
* <span data-ttu-id="11308-752">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="11308-752">Added context token to task step</span></span>
* <span data-ttu-id="11308-753">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-753">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="11308-754">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="11308-754">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-755">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-755">Appservice</span></span>
* <span data-ttu-id="11308-756">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-756">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="11308-757">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-757">Updated the default `node_version`.</span></span> <span data-ttu-id="11308-758">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-758">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="11308-759">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="11308-759">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="11308-760">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-760">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="11308-761">IotCentral</span><span class="sxs-lookup"><span data-stu-id="11308-761">IotCentral</span></span>
* <span data-ttu-id="11308-762">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="11308-762">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-763">KeyVault</span><span class="sxs-lookup"><span data-stu-id="11308-763">KeyVault</span></span>
* <span data-ttu-id="11308-764">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-764">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="11308-765">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-765">Network</span></span>
* <span data-ttu-id="11308-766">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-766">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="11308-767">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="11308-767">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="11308-768">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-768">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="11308-769">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="11308-769">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-770">Rdbms</span><span class="sxs-lookup"><span data-stu-id="11308-770">Rdbms</span></span>
* <span data-ttu-id="11308-771">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-771">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="11308-772">Rbac</span><span class="sxs-lookup"><span data-stu-id="11308-772">Rbac</span></span>
* <span data-ttu-id="11308-773">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-773">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="11308-774">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-774">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="11308-775">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-775">Storage</span></span>
* <span data-ttu-id="11308-776">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-776">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="11308-777">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-777">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="11308-778">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-778">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="11308-779">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-779">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="11308-780">VM</span><span class="sxs-lookup"><span data-stu-id="11308-780">VM</span></span>
* <span data-ttu-id="11308-781">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-781">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="11308-782">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-782">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="11308-783">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="11308-783">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="11308-784">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-784">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="11308-785">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-785">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="11308-786">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-786">Added `snapshot wait` command</span></span>
* <span data-ttu-id="11308-787">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-787">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="11308-788">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="11308-788">November 6, 2018</span></span>

<span data-ttu-id="11308-789">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="11308-789">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="11308-790">코어</span><span class="sxs-lookup"><span data-stu-id="11308-790">Core</span></span>
* <span data-ttu-id="11308-791">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-791">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="11308-792">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-792">ACR</span></span>
* <span data-ttu-id="11308-793">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-793">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="11308-794">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-794">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="11308-795">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-795">ACS</span></span>
* <span data-ttu-id="11308-796">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-796">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="11308-797">Advisor</span><span class="sxs-lookup"><span data-stu-id="11308-797">Advisor</span></span>
* <span data-ttu-id="11308-798">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-798">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="11308-799">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-799">AMS</span></span>
* <span data-ttu-id="11308-800">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="11308-800">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="11308-801">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="11308-801">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="11308-802">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-802">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="11308-803">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-803">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="11308-804">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-804">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="11308-805">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-805">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="11308-806">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-806">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="11308-807">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="11308-807">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="11308-808">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-808">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="11308-809">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-809">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="11308-810">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="11308-810">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="11308-811">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="11308-811">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="11308-812">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="11308-812">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="11308-813">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="11308-813">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="11308-814">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-814">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="11308-815">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-815">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="11308-816">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-816">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-817">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-817">AppService</span></span>
* <span data-ttu-id="11308-818">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-818">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="11308-819">구성</span><span class="sxs-lookup"><span data-stu-id="11308-819">Configure</span></span>
* <span data-ttu-id="11308-820">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-820">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="11308-821">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-821">Container</span></span>
* <span data-ttu-id="11308-822">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-822">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="11308-823">EventHub</span><span class="sxs-lookup"><span data-stu-id="11308-823">EventHub</span></span>
* <span data-ttu-id="11308-824">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-824">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-825">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-825">Interactive</span></span>
* <span data-ttu-id="11308-826">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="11308-826">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-827">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-827">Monitor</span></span>
* <span data-ttu-id="11308-828">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-828">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="11308-829">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-829">Network</span></span>
* <span data-ttu-id="11308-830">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-830">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="11308-831">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-831">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="11308-832">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-832">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="11308-833">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-833">Profile</span></span>
* <span data-ttu-id="11308-834">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-834">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-835">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-835">RDBMS</span></span>
* <span data-ttu-id="11308-836">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-836">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="11308-837">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-837">Resource</span></span>
* <span data-ttu-id="11308-838">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-838">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="11308-839">역할</span><span class="sxs-lookup"><span data-stu-id="11308-839">Role</span></span>
* <span data-ttu-id="11308-840">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-840">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="11308-841">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-841">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="11308-842">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-842">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="11308-843">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-843">Storage</span></span>
* <span data-ttu-id="11308-844">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-844">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-845">VM</span><span class="sxs-lookup"><span data-stu-id="11308-845">VM</span></span>
* <span data-ttu-id="11308-846">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-846">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="11308-847">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-847">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="11308-848">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-848">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="11308-849">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-849">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="11308-850">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="11308-850">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="11308-851">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-851">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="11308-852">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="11308-852">October 23, 2018</span></span>

<span data-ttu-id="11308-853">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="11308-853">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="11308-854">코어</span><span class="sxs-lookup"><span data-stu-id="11308-854">Core</span></span>
* <span data-ttu-id="11308-855">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-855">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="11308-856">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-856">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="11308-857">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-857">ACR</span></span>
* <span data-ttu-id="11308-858">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-858">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-859">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-859">CDN</span></span>
* <span data-ttu-id="11308-860">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-860">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="11308-861">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-861">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="11308-862">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-862">Container</span></span>
* <span data-ttu-id="11308-863">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-863">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="11308-864">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-864">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="11308-865">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-865">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="11308-866">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-866">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="11308-867">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-867">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="11308-868">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-868">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="11308-869">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-869">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-870">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-870">CosmosDB</span></span>
* <span data-ttu-id="11308-871">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-871">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-872">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-872">Interactive</span></span>
* <span data-ttu-id="11308-873">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-873">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="11308-874">IoT Central</span><span class="sxs-lookup"><span data-stu-id="11308-874">IoT Central</span></span>
* <span data-ttu-id="11308-875">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-875">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="11308-876">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-876">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-877">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-877">Monitor</span></span>
* <span data-ttu-id="11308-878">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="11308-878">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="11308-879">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-879">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="11308-880">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-880">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="11308-881">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-881">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="11308-882">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-882">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="11308-883">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-883">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="11308-884">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="11308-884">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="11308-885">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-885">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="11308-886">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-886">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="11308-887">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-887">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="11308-888">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-888">Network</span></span>
* <span data-ttu-id="11308-889">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-889">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="11308-890">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-890">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="11308-891">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11308-891">ServiceBus</span></span>
* <span data-ttu-id="11308-892">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-892">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="11308-893">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-893">SQL</span></span>
* <span data-ttu-id="11308-894">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-894">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="11308-895">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-895">Storage</span></span>
* <span data-ttu-id="11308-896">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-896">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="11308-897">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-897">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="11308-898">VM</span><span class="sxs-lookup"><span data-stu-id="11308-898">VM</span></span>
* <span data-ttu-id="11308-899">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-899">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="11308-900">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-900">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="11308-901">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-901">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="11308-902">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="11308-902">October 16, 2018</span></span>

<span data-ttu-id="11308-903">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="11308-903">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="11308-904">VM</span><span class="sxs-lookup"><span data-stu-id="11308-904">VM</span></span>
* <span data-ttu-id="11308-905">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-905">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="11308-906">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="11308-906">October 9, 2018</span></span>

<span data-ttu-id="11308-907">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="11308-907">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="11308-908">코어</span><span class="sxs-lookup"><span data-stu-id="11308-908">Core</span></span>
* <span data-ttu-id="11308-909">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="11308-909">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="11308-910">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-910">ACR</span></span>
* <span data-ttu-id="11308-911">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-911">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="11308-912">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-912">ACS</span></span>
* <span data-ttu-id="11308-913">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="11308-913">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="11308-914">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="11308-914">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="11308-915">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-915">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="11308-916">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="11308-916">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="11308-917">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-917">Container</span></span>
* <span data-ttu-id="11308-918">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-918">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="11308-919">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-919">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="11308-920">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="11308-920">Event Hub</span></span>
* <span data-ttu-id="11308-921">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-921">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="11308-922">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-922">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="11308-923">확장</span><span class="sxs-lookup"><span data-stu-id="11308-923">Extensions</span></span>
* <span data-ttu-id="11308-924">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-924">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="11308-925">HDInsight</span><span class="sxs-lookup"><span data-stu-id="11308-925">HDInsight</span></span>
* <span data-ttu-id="11308-926">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-926">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="11308-927">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-927">IoT</span></span>
* <span data-ttu-id="11308-928">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-928">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-929">KeyVault</span><span class="sxs-lookup"><span data-stu-id="11308-929">KeyVault</span></span>
* <span data-ttu-id="11308-930">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-930">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="11308-931">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-931">Network</span></span>
* <span data-ttu-id="11308-932">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-932">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="11308-933">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="11308-933">See #6052</span></span>
* <span data-ttu-id="11308-934">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="11308-934">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="11308-935">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-935">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="11308-936">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-936">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="11308-937">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-937">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="11308-938">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-938">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="11308-939">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-939">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="11308-940">역할</span><span class="sxs-lookup"><span data-stu-id="11308-940">Role</span></span>
* <span data-ttu-id="11308-941">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-941">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="11308-942">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-942">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="11308-943">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-943">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="11308-944">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-944">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="11308-945">Service Bus</span><span class="sxs-lookup"><span data-stu-id="11308-945">Service Bus</span></span>
* <span data-ttu-id="11308-946">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-946">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="11308-947">VM</span><span class="sxs-lookup"><span data-stu-id="11308-947">VM</span></span>
* <span data-ttu-id="11308-948">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-948">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="11308-949">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-949">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="11308-950">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-950">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="11308-951">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-951">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="11308-952">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-952">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="11308-953">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-953">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="11308-954">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="11308-954">September 21, 2018</span></span>

<span data-ttu-id="11308-955">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="11308-955">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="11308-956">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-956">ACR</span></span>
* <span data-ttu-id="11308-957">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-957">Added ACR Task commands</span></span>
* <span data-ttu-id="11308-958">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-958">Added quick run command</span></span>
* <span data-ttu-id="11308-959">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-959">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="11308-960">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="11308-960">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="11308-961">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-961">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="11308-962">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="11308-962">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="11308-963">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-963">ACS</span></span>
* <span data-ttu-id="11308-964">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="11308-964">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="11308-965">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="11308-965">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-966">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-966">AppService</span></span>

* <span data-ttu-id="11308-967">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-967">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="11308-968">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-968">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="11308-969">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-969">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="11308-970">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-970">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="11308-971">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-971">Batch</span></span>
* <span data-ttu-id="11308-972">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="11308-972">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="11308-973">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-973">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="11308-974">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-974">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="11308-975">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="11308-975">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="11308-976">Batch AI</span><span class="sxs-lookup"><span data-stu-id="11308-976">Batch AI</span></span> 
* <span data-ttu-id="11308-977">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="11308-977">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="11308-978">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="11308-978">Cognitive Services</span></span>
* <span data-ttu-id="11308-979">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="11308-979">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="11308-980">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-980">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="11308-981">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-981">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="11308-982">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-982">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="11308-983">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-983">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="11308-984">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-984">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="11308-985">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-985">Container</span></span>
* <span data-ttu-id="11308-986">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="11308-986">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="11308-987">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-987">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="11308-988">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-988">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="11308-989">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="11308-989">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="11308-990">Datalake</span><span class="sxs-lookup"><span data-stu-id="11308-990">Datalake</span></span>
* <span data-ttu-id="11308-991">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-991">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="11308-992">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="11308-992">Interactive Shell</span></span>
* <span data-ttu-id="11308-993">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="11308-993">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="11308-994">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-994">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="11308-995">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-995">IoT</span></span>
* <span data-ttu-id="11308-996">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-996">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="11308-997">Key Vault</span><span class="sxs-lookup"><span data-stu-id="11308-997">Key Vault</span></span>
* <span data-ttu-id="11308-998">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="11308-998">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="11308-999">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-999">Network</span></span>
* <span data-ttu-id="11308-1000">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1000">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="11308-1001">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1001">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="11308-1002">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1002">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="11308-1003">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1003">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="11308-1004">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1004">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="11308-1005">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1005">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="11308-1006">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1006">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="11308-1007">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1007">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="11308-1008">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1008">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="11308-1009">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1009">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="11308-1010">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1010">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="11308-1011">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1011">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="11308-1012">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1012">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="11308-1013">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="11308-1013">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="11308-1014">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1014">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="11308-1015">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1015">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="11308-1016">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1016">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="11308-1017">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1017">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-1018">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-1018">RDBMS</span></span>
* <span data-ttu-id="11308-1019">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1019">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="11308-1020">예약</span><span class="sxs-lookup"><span data-stu-id="11308-1020">Reservation</span></span>
* <span data-ttu-id="11308-1021">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1021">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="11308-1022">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1022">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="11308-1023">앱 관리</span><span class="sxs-lookup"><span data-stu-id="11308-1023">Manage App</span></span>
* <span data-ttu-id="11308-1024">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1024">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="11308-1025">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1025">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="11308-1026">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1026">Role</span></span>
* <span data-ttu-id="11308-1027">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1027">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="11308-1028">SignalR</span><span class="sxs-lookup"><span data-stu-id="11308-1028">SignalR</span></span>
* <span data-ttu-id="11308-1029">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1029">First release</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1030">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1030">Storage</span></span>
* <span data-ttu-id="11308-1031">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1031">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="11308-1032">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1032">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1033">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1033">VM</span></span>
* <span data-ttu-id="11308-1034">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="11308-1034">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="11308-1035">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1035">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="11308-1036">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="11308-1036">August 28, 2018</span></span>

<span data-ttu-id="11308-1037">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="11308-1037">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="11308-1038">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1038">Core</span></span>

* <span data-ttu-id="11308-1039">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1039">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="11308-1040">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1040">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1041">ACR</span></span>

* <span data-ttu-id="11308-1042">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1042">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="11308-1043">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1043">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1044">ACS</span></span>

* <span data-ttu-id="11308-1045">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1045">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="11308-1046">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1046">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1047">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1047">AppService</span></span>

* <span data-ttu-id="11308-1048">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1048">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="11308-1049">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1049">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="11308-1050">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1050">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="11308-1051">Backup</span><span class="sxs-lookup"><span data-stu-id="11308-1051">Backup</span></span>

* <span data-ttu-id="11308-1052">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1052">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="11308-1053">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="11308-1053">Bot Service</span></span>

* <span data-ttu-id="11308-1054">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1054">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="11308-1055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="11308-1055">Cognitive Services</span></span>

* <span data-ttu-id="11308-1056">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1056">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="11308-1057">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-1057">IoT</span></span>

* <span data-ttu-id="11308-1058">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1058">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1059">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1059">Monitor</span></span>

* <span data-ttu-id="11308-1060">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1060">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="11308-1061">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="11308-1061">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="11308-1062">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1062">Network</span></span>

* <span data-ttu-id="11308-1063">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1063">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1064">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1064">Resource</span></span>

* <span data-ttu-id="11308-1065">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1065">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1066">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1066">Storage</span></span>

* <span data-ttu-id="11308-1067">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1067">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1068">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1068">VM</span></span>

* <span data-ttu-id="11308-1069">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1069">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="11308-1070">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="11308-1070">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="11308-1071">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="11308-1071">Auguest 14, 2018</span></span>

<span data-ttu-id="11308-1072">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="11308-1072">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="11308-1073">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1073">Core</span></span>

* <span data-ttu-id="11308-1074">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1074">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="11308-1075">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="11308-1075">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="11308-1076">원격 분석</span><span class="sxs-lookup"><span data-stu-id="11308-1076">Telemetry</span></span>

* <span data-ttu-id="11308-1077">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="11308-1077">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1078">ACR</span></span>

* <span data-ttu-id="11308-1079">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1079">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="11308-1080">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1080">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1081">ACS</span></span>

* <span data-ttu-id="11308-1082">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1082">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="11308-1083">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1083">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="11308-1084">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1084">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="11308-1085">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1085">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="11308-1086">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1086">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="11308-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1087">AppService</span></span>

* <span data-ttu-id="11308-1088">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1088">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="11308-1089">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1089">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-1090">BatchAI</span><span class="sxs-lookup"><span data-stu-id="11308-1090">BatchAI</span></span>

* <span data-ttu-id="11308-1091">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1091">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="11308-1092">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1092">Container</span></span>

* <span data-ttu-id="11308-1093">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1093">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="11308-1094">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-1094">IoT</span></span>

* <span data-ttu-id="11308-1095">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="11308-1095">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="11308-1096">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1096">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="11308-1097">Iot Central</span><span class="sxs-lookup"><span data-stu-id="11308-1097">Iot Central</span></span>

* <span data-ttu-id="11308-1098">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1098">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-1099">KeyVault</span><span class="sxs-lookup"><span data-stu-id="11308-1099">KeyVault</span></span>


* <span data-ttu-id="11308-1100">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1100">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="11308-1101">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1101">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="11308-1102">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1102">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="11308-1103">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1103">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="11308-1104">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1104">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="11308-1105">릴레이</span><span class="sxs-lookup"><span data-stu-id="11308-1105">Relay</span></span>

* <span data-ttu-id="11308-1106">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1106">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1107">Sql</span><span class="sxs-lookup"><span data-stu-id="11308-1107">Sql</span></span>

* <span data-ttu-id="11308-1108">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1108">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1109">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1109">Storage</span></span>

* <span data-ttu-id="11308-1110">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="11308-1110">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="11308-1111">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1111">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="11308-1112">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1112">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="11308-1113">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="11308-1113">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="11308-1114">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1114">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1115">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1115">VM</span></span>

* <span data-ttu-id="11308-1116">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1116">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="11308-1117">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="11308-1117">July 31, 2018</span></span>

<span data-ttu-id="11308-1118">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="11308-1118">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1119">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1119">ACR</span></span>

* <span data-ttu-id="11308-1120">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1120">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="11308-1121">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1121">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1122">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1122">ACS</span></span>

* <span data-ttu-id="11308-1123">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1123">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1124">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1124">Batch</span></span>

* <span data-ttu-id="11308-1125">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1125">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="11308-1126">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1126">Container</span></span>

* <span data-ttu-id="11308-1127">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1127">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="11308-1128">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1128">Network</span></span>

* <span data-ttu-id="11308-1129">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1129">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="11308-1130">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1130">Resource</span></span>

* <span data-ttu-id="11308-1131">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="11308-1131">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="11308-1132">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1132">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="11308-1133">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1133">Role</span></span>

* <span data-ttu-id="11308-1134">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1134">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="11308-1135">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1135">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="11308-1136">검색</span><span class="sxs-lookup"><span data-stu-id="11308-1136">Search</span></span>

* <span data-ttu-id="11308-1137">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1137">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="11308-1138">Service Bus</span><span class="sxs-lookup"><span data-stu-id="11308-1138">Service Bus</span></span>

* <span data-ttu-id="11308-1139">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1139">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="11308-1140">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1140">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="11308-1141">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="11308-1141">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="11308-1142">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="11308-1142">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1143">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1143">Storage</span></span>

* <span data-ttu-id="11308-1144">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1144">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="11308-1145">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="11308-1145">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1146">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1146">VM</span></span>

* <span data-ttu-id="11308-1147">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1147">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="11308-1148">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1148">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="11308-1149">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1149">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="11308-1150">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1150">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="11308-1151">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="11308-1151">July 18, 2018</span></span>

<span data-ttu-id="11308-1152">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="11308-1152">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="11308-1153">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1153">Core</span></span>

* <span data-ttu-id="11308-1154">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1154">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="11308-1155">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1155">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="11308-1156">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1156">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1157">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1157">ACR</span></span>

* <span data-ttu-id="11308-1158">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1158">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="11308-1159">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1159">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="11308-1160">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1160">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="11308-1161">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1161">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1162">ACS</span></span>

* <span data-ttu-id="11308-1163">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1163">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1164">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1164">AppService</span></span>

* <span data-ttu-id="11308-1165">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1165">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1166">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1166">Batch</span></span>

* <span data-ttu-id="11308-1167">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1167">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="11308-1168">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1168">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="11308-1169">Batch AI</span><span class="sxs-lookup"><span data-stu-id="11308-1169">Batch AI</span></span>

* <span data-ttu-id="11308-1170">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1170">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="11308-1171">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1171">Container</span></span>

* <span data-ttu-id="11308-1172">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1172">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="11308-1173">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1173">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="11308-1174">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1174">Network</span></span>

* <span data-ttu-id="11308-1175">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1175">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="11308-1176">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1176">Added `network nic wait`</span></span>
* <span data-ttu-id="11308-1177">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1177">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="11308-1178">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1178">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="11308-1179">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1179">Resource</span></span>

* <span data-ttu-id="11308-1180">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1180">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="11308-1181">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1181">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="11308-1182">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1182">Added `deployment wait` command</span></span>
* <span data-ttu-id="11308-1183">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1183">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1184">SQL</span></span>

* <span data-ttu-id="11308-1185">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1185">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="11308-1186">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1186">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="11308-1187">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="11308-1187">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1188">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1188">Storage</span></span>

* <span data-ttu-id="11308-1189">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1189">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1190">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1190">VM</span></span>

* <span data-ttu-id="11308-1191">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1191">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="11308-1192">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1192">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="11308-1193">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1193">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="11308-1194">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="11308-1194">July 3, 2018</span></span>

<span data-ttu-id="11308-1195">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="11308-1195">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="11308-1196">AKS</span><span class="sxs-lookup"><span data-stu-id="11308-1196">AKS</span></span>

* <span data-ttu-id="11308-1197">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1197">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="11308-1198">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="11308-1198">July 3, 2018</span></span>

<span data-ttu-id="11308-1199">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="11308-1199">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="11308-1200">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1200">Core</span></span>

* <span data-ttu-id="11308-1201">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1201">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1202">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1202">ACR</span></span>

* <span data-ttu-id="11308-1203">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1203">Added polling build status</span></span>
* <span data-ttu-id="11308-1204">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1204">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="11308-1205">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1205">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1206">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1206">ACS</span></span>

* <span data-ttu-id="11308-1207">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1207">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="11308-1208">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1208">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="11308-1209">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="11308-1209">Updated options for `aks browse` command.</span></span> <span data-ttu-id="11308-1210">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1210">Added `--listen-port` support</span></span>
* <span data-ttu-id="11308-1211">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1211">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="11308-1212">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="11308-1212">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="11308-1213">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1213">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1214">AppService</span></span>

* <span data-ttu-id="11308-1215">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1215">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="11308-1216">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1216">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="11308-1217">Backup</span><span class="sxs-lookup"><span data-stu-id="11308-1217">Backup</span></span>

* <span data-ttu-id="11308-1218">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1218">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-1219">BatchAI</span><span class="sxs-lookup"><span data-stu-id="11308-1219">BatchAI</span></span>

* <span data-ttu-id="11308-1220">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1220">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="11308-1221">클라우드</span><span class="sxs-lookup"><span data-stu-id="11308-1221">Cloud</span></span>

* <span data-ttu-id="11308-1222">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1222">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="11308-1223">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1223">Container</span></span>

* <span data-ttu-id="11308-1224">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1224">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="11308-1225">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1225">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="11308-1226">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1226">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1227">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1227">Extension</span></span>

* <span data-ttu-id="11308-1228">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1228">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="11308-1229">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1229">Network</span></span>

* <span data-ttu-id="11308-1230">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="11308-1230">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-1231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="11308-1231">Rdbms</span></span>

* <span data-ttu-id="11308-1232">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1232">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1233">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1233">Resource</span></span>

* <span data-ttu-id="11308-1234">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1234">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1235">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1235">VM</span></span>

* <span data-ttu-id="11308-1236">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1236">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="11308-1237">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="11308-1237">June 25, 2018</span></span>

<span data-ttu-id="11308-1238">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="11308-1238">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="11308-1239">CLI</span><span class="sxs-lookup"><span data-stu-id="11308-1239">CLI</span></span>

* <span data-ttu-id="11308-1240">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1240">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="11308-1241">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="11308-1241">June 19, 2018</span></span>

<span data-ttu-id="11308-1242">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="11308-1242">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="11308-1243">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1243">Core</span></span>

* <span data-ttu-id="11308-1244">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1244">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1245">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1245">ACR</span></span>

* <span data-ttu-id="11308-1246">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1246">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="11308-1247">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1247">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1248">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1248">ACS</span></span>

* <span data-ttu-id="11308-1249">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="11308-1249">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="11308-1250">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1250">Added `--update` support</span></span>
* <span data-ttu-id="11308-1251">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1251">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="11308-1252">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="11308-1252">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="11308-1253">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1253">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="11308-1254">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1254">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="11308-1255">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1255">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="11308-1256">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1256">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1257">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1257">AppService</span></span>

* <span data-ttu-id="11308-1258">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1258">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="11308-1259">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1259">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1260">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1260">Batch</span></span>

* <span data-ttu-id="11308-1261">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1261">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="11308-1262">Batch AI</span><span class="sxs-lookup"><span data-stu-id="11308-1262">Batch AI</span></span>

* <span data-ttu-id="11308-1263">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="11308-1263">Added support for workspaces.</span></span> <span data-ttu-id="11308-1264">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1264">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="11308-1265">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="11308-1265">Added support for experiments.</span></span> <span data-ttu-id="11308-1266">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1266">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="11308-1267">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1267">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="11308-1268">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="11308-1268">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="11308-1269">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1269">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="11308-1270">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1270">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="11308-1271">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="11308-1271">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="11308-1272">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="11308-1272">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="11308-1273">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="11308-1273">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="11308-1274">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="11308-1274">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="11308-1275">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="11308-1275">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="11308-1276">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="11308-1276">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="11308-1277">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="11308-1277">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="11308-1278">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1278">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="11308-1279">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="11308-1279">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="11308-1280">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="11308-1280">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="11308-1281">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="11308-1281">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="11308-1282">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="11308-1282">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="11308-1283">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="11308-1283">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="11308-1284">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="11308-1284">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="11308-1285">지도</span><span class="sxs-lookup"><span data-stu-id="11308-1285">Maps</span></span>

* <span data-ttu-id="11308-1286">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1286">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="11308-1287">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1287">Network</span></span>

* <span data-ttu-id="11308-1288">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1288">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="11308-1289">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1289">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="11308-1290">#6502</span><span class="sxs-lookup"><span data-stu-id="11308-1290">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="11308-1291">예약</span><span class="sxs-lookup"><span data-stu-id="11308-1291">Reservations</span></span>

* <span data-ttu-id="11308-1292">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1292">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="11308-1293">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1293">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="11308-1294">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="11308-1294">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="11308-1295">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1295">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="11308-1296">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1296">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="11308-1297">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1297">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="11308-1298">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1298">Role</span></span>

* <span data-ttu-id="11308-1299">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="11308-1299">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1300">SQL</span></span>

* <span data-ttu-id="11308-1301">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1301">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1302">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1302">Storage</span></span>

* <span data-ttu-id="11308-1303">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1303">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1304">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1304">VM</span></span>

* <span data-ttu-id="11308-1305">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="11308-1305">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="11308-1306">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1306">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="11308-1307">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1307">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="11308-1308">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="11308-1308">June 13, 2018</span></span>

<span data-ttu-id="11308-1309">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="11308-1309">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="11308-1310">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1310">Core</span></span>

* <span data-ttu-id="11308-1311">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="11308-1311">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="11308-1312">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="11308-1312">June 13, 2018</span></span>

<span data-ttu-id="11308-1313">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="11308-1313">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="11308-1314">AKS</span><span class="sxs-lookup"><span data-stu-id="11308-1314">AKS</span></span>

* <span data-ttu-id="11308-1315">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1315">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="11308-1316">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="11308-1316">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="11308-1317">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1317">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="11308-1318">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1318">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="11308-1319">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1319">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1320">AppService</span></span>

* <span data-ttu-id="11308-1321">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1321">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="11308-1322">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="11308-1322">June 5, 2018</span></span>

<span data-ttu-id="11308-1323">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="11308-1323">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1324">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1324">Interactive</span></span>

* <span data-ttu-id="11308-1325">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1325">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="11308-1326">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="11308-1326">June 5, 2018</span></span>

<span data-ttu-id="11308-1327">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="11308-1327">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="11308-1328">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1328">Core</span></span>

* <span data-ttu-id="11308-1329">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1329">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="11308-1330">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1330">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1331">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1331">ACR</span></span>

* <span data-ttu-id="11308-1332">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1332">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="11308-1333">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1333">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="11308-1334">AKS</span><span class="sxs-lookup"><span data-stu-id="11308-1334">AKS</span></span>

* <span data-ttu-id="11308-1335">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1335">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1336">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1336">Batch</span></span>

* <span data-ttu-id="11308-1337">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="11308-1337">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="11308-1338">IOT</span><span class="sxs-lookup"><span data-stu-id="11308-1338">IOT</span></span>

* <span data-ttu-id="11308-1339">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1339">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="11308-1340">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1340">Network</span></span>

* <span data-ttu-id="11308-1341">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="11308-1341">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="11308-1342">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="11308-1342">Policy Insights</span></span>

* <span data-ttu-id="11308-1343">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1343">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="11308-1344">ARM</span><span class="sxs-lookup"><span data-stu-id="11308-1344">ARM</span></span>

* <span data-ttu-id="11308-1345">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1345">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1346">SQL</span></span>

* <span data-ttu-id="11308-1347">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="11308-1347">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="11308-1348">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1348">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="11308-1349">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1349">Storage</span></span>

* <span data-ttu-id="11308-1350">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="11308-1350">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1351">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1351">VM</span></span>

* <span data-ttu-id="11308-1352">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1352">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="11308-1353">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1353">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="11308-1354">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1354">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="11308-1355">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="11308-1355">May 22, 2018</span></span>

<span data-ttu-id="11308-1356">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="11308-1356">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="11308-1357">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1357">Core</span></span>

* <span data-ttu-id="11308-1358">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1358">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1359">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1359">ACS</span></span>

* <span data-ttu-id="11308-1360">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1360">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="11308-1361">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1361">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1362">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-1362">AppService</span></span>

* <span data-ttu-id="11308-1363">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1363">Improved generic update commands</span></span>
* <span data-ttu-id="11308-1364">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1364">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="11308-1365">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1365">Container</span></span>

* <span data-ttu-id="11308-1366">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1366">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="11308-1367">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1367">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1368">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1368">Extension</span></span>

* <span data-ttu-id="11308-1369">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1369">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1370">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1370">Interactive</span></span>

* <span data-ttu-id="11308-1371">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1371">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="11308-1372">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1372">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-1373">KeyVault</span><span class="sxs-lookup"><span data-stu-id="11308-1373">KeyVault</span></span>

* <span data-ttu-id="11308-1374">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="11308-1374">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="11308-1375">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1375">Network</span></span>

* <span data-ttu-id="11308-1376">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1376">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="11308-1377">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1377">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1378">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1378">SQL</span></span>

* <span data-ttu-id="11308-1379">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="11308-1379">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="11308-1380">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="11308-1380">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="11308-1381">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1381">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="11308-1382">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1382">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="11308-1383">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1383">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="11308-1384">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="11308-1384">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="11308-1385">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1385">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="11308-1386">`edition`.</span><span class="sxs-lookup"><span data-stu-id="11308-1386">`edition`.</span></span> <span data-ttu-id="11308-1387">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1387">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="11308-1388">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="11308-1388">`elasticPoolName`.</span></span> <span data-ttu-id="11308-1389">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1389">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="11308-1390">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1390">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="11308-1391">`edition`.</span><span class="sxs-lookup"><span data-stu-id="11308-1391">`edition`.</span></span> <span data-ttu-id="11308-1392">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="11308-1392">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="11308-1393">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="11308-1393">`dtu`.</span></span> <span data-ttu-id="11308-1394">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="11308-1394">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="11308-1395">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="11308-1395">`databaseDtuMin`.</span></span> <span data-ttu-id="11308-1396">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="11308-1396">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="11308-1397">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="11308-1397">`databaseDtuMax`.</span></span> <span data-ttu-id="11308-1398">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="11308-1398">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="11308-1399">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1399">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="11308-1400">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1400">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1401">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1401">Storage</span></span>

* <span data-ttu-id="11308-1402">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1402">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="11308-1403">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1403">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1404">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1404">VM</span></span>

* <span data-ttu-id="11308-1405">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="11308-1405">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="11308-1406">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-1406">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="11308-1407">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1407">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="11308-1408">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1408">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="11308-1409">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1409">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="11308-1410">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="11308-1410">May 7, 2018</span></span>

<span data-ttu-id="11308-1411">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="11308-1411">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="11308-1412">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1412">Core</span></span>

* <span data-ttu-id="11308-1413">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1413">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="11308-1414">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1414">Added limited support for positional arguments</span></span>
* <span data-ttu-id="11308-1415">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1415">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="11308-1416">#5591</span><span class="sxs-lookup"><span data-stu-id="11308-1416">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="11308-1417">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1417">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="11308-1418">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1418">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="11308-1419">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1419">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="11308-1420">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1420">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="11308-1421">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1421">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1422">ACR</span></span>

* <span data-ttu-id="11308-1423">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1423">Added ACR Build commands</span></span>
* <span data-ttu-id="11308-1424">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1424">Improved resource not found error messages</span></span>
* <span data-ttu-id="11308-1425">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1425">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="11308-1426">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1426">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="11308-1427">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1427">Improved repository commands error messages</span></span>
* <span data-ttu-id="11308-1428">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1428">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1429">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1429">ACS</span></span>

* <span data-ttu-id="11308-1430">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1430">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="11308-1431">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1431">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="11308-1432">AMS</span><span class="sxs-lookup"><span data-stu-id="11308-1432">AMS</span></span>

* <span data-ttu-id="11308-1433">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="11308-1433">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1434">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1434">Appservice</span></span>

* <span data-ttu-id="11308-1435">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1435">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="11308-1436">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1436">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="11308-1437">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1437">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="11308-1438">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1438">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="11308-1439">Batch AI</span><span class="sxs-lookup"><span data-stu-id="11308-1439">Batch AI</span></span>

* <span data-ttu-id="11308-1440">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1440">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="11308-1441">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="11308-1441">Cognitive Services</span></span>

* <span data-ttu-id="11308-1442">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1442">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-1443">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-1443">Consumption</span></span>

* <span data-ttu-id="11308-1444">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1444">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="11308-1445">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1445">Container</span></span>

* <span data-ttu-id="11308-1446">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1446">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="11308-1447">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="11308-1447">Cosmos DB</span></span>

* <span data-ttu-id="11308-1448">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="11308-1448">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="11308-1449">DMS</span><span class="sxs-lookup"><span data-stu-id="11308-1449">DMS</span></span>

* <span data-ttu-id="11308-1450">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1450">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1451">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1451">Extension</span></span>

* <span data-ttu-id="11308-1452">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1452">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1453">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1453">Interactive</span></span>

* <span data-ttu-id="11308-1454">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1454">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="11308-1455">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="11308-1455">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="11308-1456">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1456">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="11308-1457">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1457">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="11308-1458">랩</span><span class="sxs-lookup"><span data-stu-id="11308-1458">Lab</span></span>

* <span data-ttu-id="11308-1459">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1459">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="11308-1460">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1460">Network</span></span>

* <span data-ttu-id="11308-1461">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1461">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="11308-1462">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1462">Profile</span></span>

* <span data-ttu-id="11308-1463">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1463">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="11308-1464">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1464">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="11308-1465">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1465">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="11308-1466">Redis</span><span class="sxs-lookup"><span data-stu-id="11308-1466">Redis</span></span>

* <span data-ttu-id="11308-1467">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-1467">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="11308-1468">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1468">Deprecated `redis list-all`.</span></span> <span data-ttu-id="11308-1469">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="11308-1469">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="11308-1470">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-1470">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="11308-1471">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1471">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="11308-1472">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1472">Role</span></span>

* <span data-ttu-id="11308-1473">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1473">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1474">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1474">Storage</span></span>

* <span data-ttu-id="11308-1475">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1475">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="11308-1476">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="11308-1476">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="11308-1477">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="11308-1477">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="11308-1478">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1478">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="11308-1479">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1479">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1480">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1480">VM</span></span>

* <span data-ttu-id="11308-1481">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1481">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="11308-1482">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1482">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="11308-1483">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="11308-1483">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="11308-1484">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1484">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="11308-1485">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1485">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="11308-1486">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1486">Added write accelerator support</span></span>
* <span data-ttu-id="11308-1487">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1487">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="11308-1488">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1488">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="11308-1489">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1489">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="11308-1490">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="11308-1490">April 10, 2018</span></span>

<span data-ttu-id="11308-1491">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="11308-1491">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1492">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1492">ACR</span></span>

* <span data-ttu-id="11308-1493">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="11308-1493">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1494">ACS</span></span>

* <span data-ttu-id="11308-1495">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1495">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1496">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1496">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="11308-1498">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1498">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-1499">BatchAI</span><span class="sxs-lookup"><span data-stu-id="11308-1499">BatchAI</span></span>

* <span data-ttu-id="11308-1500">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1500">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="11308-1501">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="11308-1501">Job level mounting</span></span>
  - <span data-ttu-id="11308-1502">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="11308-1502">Environment variables with secret values</span></span>
  - <span data-ttu-id="11308-1503">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1503">Performance counters settings</span></span>
  - <span data-ttu-id="11308-1504">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="11308-1504">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="11308-1505">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1505">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="11308-1506">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="11308-1506">Usage and limits reporting</span></span>
  - <span data-ttu-id="11308-1507">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1507">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="11308-1508">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1508">Support for custom images</span></span>
  - <span data-ttu-id="11308-1509">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1509">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="11308-1510">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1510">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="11308-1511">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1511">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="11308-1512">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-1512">National clouds are supported</span></span>
* <span data-ttu-id="11308-1513">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1513">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="11308-1514">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="11308-1514">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="11308-1515">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1515">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="11308-1516">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1516">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="11308-1517">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="11308-1517">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="11308-1518">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="11308-1518">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="11308-1519">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1519">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="11308-1520">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1520">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="11308-1521">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1521">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="11308-1522">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1522">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="11308-1523">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1523">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="11308-1524">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="11308-1524">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="11308-1525">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1525">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="11308-1526">결제</span><span class="sxs-lookup"><span data-stu-id="11308-1526">Billing</span></span>

* <span data-ttu-id="11308-1527">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1527">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-1528">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-1528">Consumption</span></span>

* <span data-ttu-id="11308-1529">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1529">Added `marketplace` commands</span></span>
* <span data-ttu-id="11308-1530">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1530">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="11308-1531">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1531">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="11308-1532">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1532">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="11308-1533">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1533">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="11308-1534">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1534">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="11308-1535">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1535">Container</span></span>

* <span data-ttu-id="11308-1536">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="11308-1536">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="11308-1537">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="11308-1537">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1538">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1538">Extension</span></span>

* <span data-ttu-id="11308-1539">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1539">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1540">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1540">Interactive</span></span>

* <span data-ttu-id="11308-1541">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1541">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="11308-1542">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1542">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="11308-1543">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1543">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="11308-1544">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1544">Network</span></span>

* <span data-ttu-id="11308-1545">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1545">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="11308-1546">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1546">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="11308-1547">#4910</span><span class="sxs-lookup"><span data-stu-id="11308-1547">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="11308-1548">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1548">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="11308-1549">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="11308-1549">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="11308-1550">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1550">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="11308-1551">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1551">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="11308-1552">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1552">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-1553">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1553">Profile</span></span>

* <span data-ttu-id="11308-1554">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1554">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="11308-1555">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1555">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-1556">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-1556">RDBMS</span></span>

* <span data-ttu-id="11308-1557">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1557">Added `georestore` command</span></span>
* <span data-ttu-id="11308-1558">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1558">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1559">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1559">Resource</span></span>

* <span data-ttu-id="11308-1560">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1560">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="11308-1561">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1561">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1562">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1562">SQL</span></span>

* <span data-ttu-id="11308-1563">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1563">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1564">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1564">Storage</span></span>

* <span data-ttu-id="11308-1565">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1565">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1566">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1566">VM</span></span>

* <span data-ttu-id="11308-1567">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1567">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="11308-1568">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1568">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="11308-1570">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1570">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="11308-1571">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1571">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="11308-1572">#5718</span><span class="sxs-lookup"><span data-stu-id="11308-1572">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="11308-1573">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1573">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="11308-1574">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="11308-1574">March 27, 2018</span></span>

<span data-ttu-id="11308-1575">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="11308-1575">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="11308-1576">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1576">Core</span></span>

* <span data-ttu-id="11308-1577">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="11308-1577">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1578">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1578">ACS</span></span>

* <span data-ttu-id="11308-1579">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1579">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1580">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1580">Appservice</span></span>

* <span data-ttu-id="11308-1581">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1581">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="11308-1582">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1582">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="11308-1583">Backup</span><span class="sxs-lookup"><span data-stu-id="11308-1583">Backup</span></span>

* <span data-ttu-id="11308-1584">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1584">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="11308-1585">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1585">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="11308-1586">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1586">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="11308-1587">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1587">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="11308-1588">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1588">Container</span></span>

* <span data-ttu-id="11308-1589">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1589">Added `container exec` command.</span></span> <span data-ttu-id="11308-1590">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1590">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="11308-1591">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="11308-1591">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1592">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1592">Extension</span></span>

* <span data-ttu-id="11308-1593">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1593">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="11308-1594">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1594">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="11308-1595">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1595">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1596">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1596">Interactive</span></span>

* <span data-ttu-id="11308-1597">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="11308-1597">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="11308-1598">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1598">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="11308-1599">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="11308-1599">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="11308-1600">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1600">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="11308-1601">랩</span><span class="sxs-lookup"><span data-stu-id="11308-1601">Lab</span></span>

* <span data-ttu-id="11308-1602">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1602">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1603">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1603">Monitor</span></span>

* <span data-ttu-id="11308-1604">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1604">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="11308-1605">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="11308-1605">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="11308-1606">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1606">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="11308-1607">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1607">Network</span></span>

* <span data-ttu-id="11308-1608">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1608">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="11308-1609">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1609">Profile</span></span>

* <span data-ttu-id="11308-1610">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1610">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-1611">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-1611">RDBMS</span></span>

* <span data-ttu-id="11308-1612">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1612">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1613">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1613">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="11308-1615">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1615">Role</span></span>

* <span data-ttu-id="11308-1616">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1616">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="11308-1617">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1617">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="11308-1618">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1618">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="11308-1619">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1619">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="11308-1620">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1620">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1621">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1621">Storage</span></span>

* <span data-ttu-id="11308-1622">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1622">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="11308-1623">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="11308-1623">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1624">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1624">VM</span></span>

* <span data-ttu-id="11308-1625">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1625">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="11308-1626">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1626">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="11308-1627">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1627">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="11308-1628">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1628">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="11308-1629">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="11308-1629">March 13, 2018</span></span>

<span data-ttu-id="11308-1630">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="11308-1630">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1631">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1631">ACR</span></span>

* <span data-ttu-id="11308-1632">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1632">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="11308-1633">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1633">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="11308-1634">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1634">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1635">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1635">ACS</span></span>

* <span data-ttu-id="11308-1636">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1636">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="11308-1637">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1637">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="11308-1638">Advisor</span><span class="sxs-lookup"><span data-stu-id="11308-1638">Advisor</span></span>

* <span data-ttu-id="11308-1639">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1639">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="11308-1640">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1640">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="11308-1641">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1641">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="11308-1642">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1642">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="11308-1643">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1643">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1644">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1644">Appservice</span></span>

* <span data-ttu-id="11308-1645">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1645">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="11308-1646">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1646">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="11308-1647">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="11308-1647">Eventhubs</span></span>

* <span data-ttu-id="11308-1648">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1648">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1649">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1649">Extension</span></span>

* <span data-ttu-id="11308-1650">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1650">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1651">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1651">Interactive</span></span>

* <span data-ttu-id="11308-1652">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="11308-1652">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="11308-1653">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="11308-1653">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="11308-1654">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1654">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="11308-1655">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1655">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1656">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1656">Monitor</span></span>

* <span data-ttu-id="11308-1657">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1657">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="11308-1658">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1658">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="11308-1659">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1659">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="11308-1660">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1660">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="11308-1661">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1661">Network</span></span>

* <span data-ttu-id="11308-1662">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1662">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="11308-1663">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="11308-1663">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="11308-1664">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1664">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="11308-1665">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1665">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-1666">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1666">Profile</span></span>

* <span data-ttu-id="11308-1667">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1667">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="11308-1668">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1668">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-1669">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-1669">RDBMS</span></span>

* <span data-ttu-id="11308-1670">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1670">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="11308-1671">Service Bus</span><span class="sxs-lookup"><span data-stu-id="11308-1671">Service Bus</span></span>

* <span data-ttu-id="11308-1672">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1672">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1673">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1673">Storage</span></span>

* <span data-ttu-id="11308-1674">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1674">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="11308-1675">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1675">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1676">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1676">VM</span></span>

* <span data-ttu-id="11308-1677">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1677">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="11308-1678">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-1678">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="11308-1679">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1679">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="11308-1680">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1680">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="11308-1681">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="11308-1681">February 27, 2018</span></span>

<span data-ttu-id="11308-1682">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="11308-1682">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="11308-1683">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1683">Core</span></span>

* <span data-ttu-id="11308-1684">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="11308-1684">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="11308-1685">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1685">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="11308-1686">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1686">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1687">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1687">ACS</span></span>

* <span data-ttu-id="11308-1688">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1688">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="11308-1689">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="11308-1689">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="11308-1690">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1690">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="11308-1691">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1691">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1692">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1692">Appservice</span></span>

* <span data-ttu-id="11308-1693">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="11308-1693">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="11308-1694">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1694">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="11308-1695">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="11308-1695">Cognitive Services</span></span>

* <span data-ttu-id="11308-1696">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1696">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-1697">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-1697">Consumption</span></span>

* <span data-ttu-id="11308-1698">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1698">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="11308-1699">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1699">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="11308-1700">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1700">Container</span></span>

* <span data-ttu-id="11308-1701">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1701">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="11308-1702">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1702">Network</span></span>

* <span data-ttu-id="11308-1703">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="11308-1703">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1704">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1704">Resource</span></span>

* <span data-ttu-id="11308-1705">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1705">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="11308-1706">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1706">Role</span></span>

* <span data-ttu-id="11308-1707">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1707">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1708">SQL</span></span>

* <span data-ttu-id="11308-1709">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1709">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1710">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1710">Storage</span></span>

* <span data-ttu-id="11308-1711">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="11308-1711">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1712">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1712">VM</span></span>

* <span data-ttu-id="11308-1713">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1713">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="11308-1714">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="11308-1714">February 13, 2018</span></span>

<span data-ttu-id="11308-1715">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="11308-1715">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="11308-1716">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1716">Core</span></span>

* <span data-ttu-id="11308-1717">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1717">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1718">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1718">ACS</span></span>

* <span data-ttu-id="11308-1719">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1719">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="11308-1720">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1720">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="11308-1721">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1721">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="11308-1722">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="11308-1722">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="11308-1723">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1723">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="11308-1724">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="11308-1724">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="11308-1725">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1725">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="11308-1726">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1726">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1727">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1727">Appservice</span></span>

* <span data-ttu-id="11308-1728">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1728">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="11308-1729">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1729">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-1730">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-1730">CDN</span></span>

* <span data-ttu-id="11308-1731">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1731">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="11308-1732">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1732">Container</span></span>

* <span data-ttu-id="11308-1733">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1733">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="11308-1734">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1734">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-1735">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-1735">CosmosDB</span></span>

* <span data-ttu-id="11308-1736">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1736">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1737">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1737">Extension</span></span>

* <span data-ttu-id="11308-1738">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1738">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="11308-1739">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1739">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="11308-1740">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="11308-1740">Feedback</span></span>

* <span data-ttu-id="11308-1741">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1741">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1742">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1742">Interactive</span></span>

* <span data-ttu-id="11308-1743">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1743">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="11308-1744">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1744">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="11308-1745">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-1745">IoT</span></span>

* <span data-ttu-id="11308-1746">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1746">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="11308-1747">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1747">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="11308-1748">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1748">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="11308-1749">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1749">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1750">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1750">Monitor</span></span>

* <span data-ttu-id="11308-1751">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1751">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="11308-1752">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1752">Network</span></span>

* <span data-ttu-id="11308-1753">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1753">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="11308-1754">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1754">Profile</span></span>

* <span data-ttu-id="11308-1755">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1755">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1756">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1756">Resource</span></span>

* <span data-ttu-id="11308-1757">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1757">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="11308-1758">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1758">Role</span></span>

* <span data-ttu-id="11308-1759">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1759">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1760">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1760">SQL</span></span>

* <span data-ttu-id="11308-1761">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1761">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="11308-1762">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1762">Added `sql db rename`</span></span>
* <span data-ttu-id="11308-1763">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1763">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1764">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1764">Storage</span></span>

* <span data-ttu-id="11308-1765">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1765">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1766">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1766">VM</span></span>

* <span data-ttu-id="11308-1767">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1767">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="11308-1768">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1768">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="11308-1769">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="11308-1769">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="11308-1770">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="11308-1770">January 31, 2018</span></span>

<span data-ttu-id="11308-1771">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="11308-1771">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="11308-1772">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1772">Core</span></span>

* <span data-ttu-id="11308-1773">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1773">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="11308-1774">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1774">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="11308-1775">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1775">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="11308-1776">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="11308-1776">Use `--verbose` to see</span></span>
* <span data-ttu-id="11308-1777">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1777">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1778">ACS</span></span>

* <span data-ttu-id="11308-1779">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1779">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="11308-1780">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="11308-1780">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1781">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1781">Appservice</span></span>

* <span data-ttu-id="11308-1782">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="11308-1782">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="11308-1783">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="11308-1783">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-1784">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-1784">CDN</span></span>

* <span data-ttu-id="11308-1785">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1785">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-1786">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-1786">CosmosDB</span></span>

* <span data-ttu-id="11308-1787">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1787">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1788">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1788">Interactive</span></span>

* <span data-ttu-id="11308-1789">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1789">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="11308-1790">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1790">Network</span></span>

* <span data-ttu-id="11308-1791">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1791">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="11308-1792">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1792">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="11308-1793">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1793">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="11308-1794">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1794">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="11308-1795">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1795">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="11308-1796">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="11308-1796">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="11308-1797">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1797">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="11308-1798">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1798">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="11308-1799">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1799">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="11308-1800">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="11308-1800">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="11308-1801">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1801">Profile</span></span>

* <span data-ttu-id="11308-1802">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1802">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1803">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1803">Resource</span></span>

* <span data-ttu-id="11308-1804">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1804">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1805">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1805">Storage</span></span>

* <span data-ttu-id="11308-1806">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1806">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="11308-1807">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1807">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="11308-1808">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1808">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="11308-1809">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1809">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="11308-1810">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1810">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1811">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1811">VM</span></span>

* <span data-ttu-id="11308-1812">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1812">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="11308-1813">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1813">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="11308-1814">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1814">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="11308-1815">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1815">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="11308-1816">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="11308-1816">January 17, 2018</span></span>

<span data-ttu-id="11308-1817">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="11308-1817">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1818">ACR</span></span>

* <span data-ttu-id="11308-1819">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1819">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="11308-1820">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1820">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1821">ACS</span></span>

* <span data-ttu-id="11308-1822">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1822">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="11308-1823">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1823">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1824">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1824">Appservice</span></span>

* <span data-ttu-id="11308-1825">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1825">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="11308-1826">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1826">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="11308-1827">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1827">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="11308-1828">Backup</span><span class="sxs-lookup"><span data-stu-id="11308-1828">Backup</span></span>

* <span data-ttu-id="11308-1829">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1829">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="11308-1830">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1830">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="11308-1831">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1831">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="11308-1832">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1832">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="11308-1833">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1833">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1834">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1834">Batch</span></span>

* <span data-ttu-id="11308-1835">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1835">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="11308-1836">클라우드</span><span class="sxs-lookup"><span data-stu-id="11308-1836">Cloud</span></span>

* <span data-ttu-id="11308-1837">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1837">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-1838">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-1838">Consumption</span></span>

* <span data-ttu-id="11308-1839">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1839">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="11308-1840">Event Grid</span><span class="sxs-lookup"><span data-stu-id="11308-1840">Event Grid</span></span>

* <span data-ttu-id="11308-1841">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="11308-1841">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="11308-1842">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="11308-1842">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="11308-1843">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1843">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="11308-1844">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="11308-1844">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="11308-1845">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1845">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="11308-1846">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1846">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="11308-1847">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1847">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="11308-1848">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1848">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-1849">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-1849">Interactive</span></span>

* <span data-ttu-id="11308-1850">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1850">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="11308-1851">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1851">Fixed errors on startup</span></span>
* <span data-ttu-id="11308-1852">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1852">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="11308-1853">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-1853">IoT</span></span>

* <span data-ttu-id="11308-1854">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1854">Added support for device provisioning service</span></span>
* <span data-ttu-id="11308-1855">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1855">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="11308-1856">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1856">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1857">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1857">Monitor</span></span>

* <span data-ttu-id="11308-1858">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1858">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="11308-1859">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="11308-1859">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="11308-1860">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1860">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="11308-1861">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1861">Network</span></span>

* <span data-ttu-id="11308-1862">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1862">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="11308-1863">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1863">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-1864">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-1864">Profile</span></span>

* <span data-ttu-id="11308-1865">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1865">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="11308-1866">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1866">Role</span></span>

* <span data-ttu-id="11308-1867">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1867">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="11308-1868">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="11308-1868">Service Fabric</span></span>

* <span data-ttu-id="11308-1869">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1869">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="11308-1870">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1870">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1871">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1871">VM</span></span>

* <span data-ttu-id="11308-1872">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="11308-1872">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="11308-1873">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1873">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="11308-1874">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1874">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="11308-1875">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1875">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="11308-1876">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1876">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="11308-1877">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1877">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="11308-1878">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1878">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="11308-1879">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1879">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="11308-1880">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="11308-1880">December 19, 2017</span></span>

<span data-ttu-id="11308-1881">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="11308-1881">Version 2.0.23</span></span>

* <span data-ttu-id="11308-1882">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1882">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="11308-1883">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1883">Container</span></span>

* <span data-ttu-id="11308-1884">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1884">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="11308-1885">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1885">Network</span></span>

* <span data-ttu-id="11308-1886">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1886">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="11308-1887">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1887">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1888">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1888">Storage</span></span>

* <span data-ttu-id="11308-1889">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1889">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1890">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1890">VM</span></span>

* <span data-ttu-id="11308-1891">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1891">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="11308-1892">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="11308-1892">December 5, 2017</span></span>

<span data-ttu-id="11308-1893">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="11308-1893">Version 2.0.22</span></span>

* <span data-ttu-id="11308-1894">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-1894">Removed `az component` commands.</span></span> <span data-ttu-id="11308-1895">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="11308-1895">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="11308-1896">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1896">Core</span></span>
* <span data-ttu-id="11308-1897">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1897">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="11308-1898">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1898">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="11308-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1899">ACS</span></span>

* <span data-ttu-id="11308-1900">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1900">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="11308-1901">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1901">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="11308-1902">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1902">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="11308-1903">Advisor</span><span class="sxs-lookup"><span data-stu-id="11308-1903">Advisor</span></span>

* <span data-ttu-id="11308-1904">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1904">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1905">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1905">Appservice</span></span>

* <span data-ttu-id="11308-1906">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-1906">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="11308-1907">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1907">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="11308-1908">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1908">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="11308-1909">Consumption</span><span class="sxs-lookup"><span data-stu-id="11308-1909">Consumption</span></span>

* <span data-ttu-id="11308-1910">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1910">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="11308-1911">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1911">Container</span></span>

* <span data-ttu-id="11308-1912">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1912">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1913">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1913">Monitor</span></span>

* <span data-ttu-id="11308-1914">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1914">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1915">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1915">Resource</span></span>

* <span data-ttu-id="11308-1916">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1916">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="11308-1917">역할</span><span class="sxs-lookup"><span data-stu-id="11308-1917">Role</span></span>

* <span data-ttu-id="11308-1918">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1918">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="11308-1919">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1919">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="11308-1920">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="11308-1920">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1921">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1921">SQL</span></span>

* <span data-ttu-id="11308-1922">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1922">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="11308-1923">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1923">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1924">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1924">VM</span></span>

* <span data-ttu-id="11308-1925">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1925">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="11308-1926">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="11308-1926">November 14, 2017</span></span>

<span data-ttu-id="11308-1927">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="11308-1927">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1928">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1928">ACR</span></span>

* <span data-ttu-id="11308-1929">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1929">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="11308-1930">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-1930">ACS</span></span>

* <span data-ttu-id="11308-1931">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1931">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="11308-1932">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="11308-1932">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="11308-1933">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1933">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="11308-1934">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1934">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="11308-1935">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1935">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-1936">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-1936">Appservice</span></span>

* <span data-ttu-id="11308-1937">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1937">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="11308-1938">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1938">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="11308-1939">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-1939">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="11308-1940">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-1940">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="11308-1941">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1941">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="11308-1942">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="11308-1942">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="11308-1943">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-1943">Batch</span></span>

* <span data-ttu-id="11308-1944">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1944">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-1945">Batchai</span><span class="sxs-lookup"><span data-stu-id="11308-1945">Batchai</span></span>

* <span data-ttu-id="11308-1946">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1946">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="11308-1947">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1947">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="11308-1948">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1948">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="11308-1949">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1949">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="11308-1950">클라우드</span><span class="sxs-lookup"><span data-stu-id="11308-1950">Cloud</span></span>

* <span data-ttu-id="11308-1951">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1951">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="11308-1952">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-1952">Container</span></span>

* <span data-ttu-id="11308-1953">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1953">Added support to open multiple ports</span></span>
* <span data-ttu-id="11308-1954">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1954">Added container group restart policy</span></span>
* <span data-ttu-id="11308-1955">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1955">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="11308-1956">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="11308-1956">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="11308-1957">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="11308-1957">Data Lake Analytics</span></span>

* <span data-ttu-id="11308-1958">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1958">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="11308-1959">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="11308-1959">Data Lake Store</span></span>

* <span data-ttu-id="11308-1960">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1960">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="11308-1961">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-1961">Extension</span></span>

* <span data-ttu-id="11308-1962">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1962">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="11308-1963">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1963">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="11308-1964">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-1964">IoT</span></span>

* <span data-ttu-id="11308-1965">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1965">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-1966">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-1966">Monitor</span></span>

* <span data-ttu-id="11308-1967">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1967">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="11308-1968">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-1968">Network</span></span>

* <span data-ttu-id="11308-1969">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1969">Added support for CAA DNS records</span></span>
* <span data-ttu-id="11308-1970">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1970">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="11308-1971">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1971">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="11308-1972">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1972">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="11308-1973">예약</span><span class="sxs-lookup"><span data-stu-id="11308-1973">Reservations</span></span>

* <span data-ttu-id="11308-1974">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-1974">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="11308-1975">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-1975">Resource</span></span>

* <span data-ttu-id="11308-1976">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1976">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="11308-1977">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-1977">SQL</span></span>

* <span data-ttu-id="11308-1978">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-1978">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-1979">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-1979">Storage</span></span>

* <span data-ttu-id="11308-1980">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="11308-1980">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="11308-1981">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-1981">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="11308-1982">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1982">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="11308-1983">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="11308-1983">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="11308-1984">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1984">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="11308-1985">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1985">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="11308-1986">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-1986">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="11308-1987">VM</span><span class="sxs-lookup"><span data-stu-id="11308-1987">VM</span></span>

* <span data-ttu-id="11308-1988">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-1988">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="11308-1989">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1989">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="11308-1990">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1990">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="11308-1991">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-1991">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="11308-1992">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-1992">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="11308-1993">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="11308-1993">October 24, 2017</span></span>

<span data-ttu-id="11308-1994">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="11308-1994">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="11308-1995">코어</span><span class="sxs-lookup"><span data-stu-id="11308-1995">Core</span></span>

* <span data-ttu-id="11308-1996">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="11308-1996">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="11308-1997">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-1997">ACR</span></span>

* <span data-ttu-id="11308-1998">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="11308-1998">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="11308-1999">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-1999">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="11308-2000">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="11308-2000">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2001">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2001">ACS</span></span>

* <span data-ttu-id="11308-2002">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2002">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="11308-2003">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2003">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2004">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2004">Appservice</span></span>

* <span data-ttu-id="11308-2005">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="11308-2005">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="11308-2006">구성 요소</span><span class="sxs-lookup"><span data-stu-id="11308-2006">Component</span></span>

* <span data-ttu-id="11308-2007">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2007">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-2008">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-2008">Monitor</span></span>

* <span data-ttu-id="11308-2009">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2009">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2010">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2010">Resource</span></span>

* <span data-ttu-id="11308-2011">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2011">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="11308-2012">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2012">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2013">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2013">VM</span></span>

* <span data-ttu-id="11308-2014">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2014">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="11308-2015">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="11308-2015">October 9, 2017</span></span>

<span data-ttu-id="11308-2016">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="11308-2016">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="11308-2017">코어</span><span class="sxs-lookup"><span data-stu-id="11308-2017">Core</span></span>

* <span data-ttu-id="11308-2018">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2018">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2019">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2019">Appservice</span></span>

* <span data-ttu-id="11308-2020">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2020">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="11308-2021">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-2021">Batch</span></span>

* <span data-ttu-id="11308-2022">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2022">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="11308-2023">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2023">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="11308-2024">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2024">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="11308-2025">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2025">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="11308-2026">Batchai</span><span class="sxs-lookup"><span data-stu-id="11308-2026">Batchai</span></span>

* <span data-ttu-id="11308-2027">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2027">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-2028">Keyvault</span><span class="sxs-lookup"><span data-stu-id="11308-2028">Keyvault</span></span>

* <span data-ttu-id="11308-2029">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2029">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="11308-2030">(#4448)</span><span class="sxs-lookup"><span data-stu-id="11308-2030">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="11308-2031">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2031">Network</span></span>

* <span data-ttu-id="11308-2032">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2032">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="11308-2033">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2033">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2034">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2034">Resource</span></span>

* <span data-ttu-id="11308-2035">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2035">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="11308-2036">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2036">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="11308-2037">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2037">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="11308-2038">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2038">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="11308-2039">Sql</span><span class="sxs-lookup"><span data-stu-id="11308-2039">Sql</span></span>

* <span data-ttu-id="11308-2040">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2040">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="11308-2041">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2041">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="11308-2042">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2042">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2043">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2043">Storage</span></span>

* <span data-ttu-id="11308-2044">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2044">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2045">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2045">Vm</span></span>

* <span data-ttu-id="11308-2046">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2046">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="11308-2047">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2047">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="11308-2048">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2048">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="11308-2049">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2049">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="11308-2050">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2050">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="11308-2051">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="11308-2051">September 22, 2017</span></span>

<span data-ttu-id="11308-2052">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="11308-2052">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2053">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2053">Resource</span></span>

* <span data-ttu-id="11308-2054">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2054">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="11308-2055">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2055">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="11308-2056">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2056">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="11308-2057">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2057">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="11308-2058">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2058">Network</span></span>

* <span data-ttu-id="11308-2059">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2059">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="11308-2060">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2060">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="11308-2061">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2061">Added `asg` application security group commands</span></span>
* <span data-ttu-id="11308-2062">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2062">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="11308-2063">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2063">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="11308-2064">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2064">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="11308-2065">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2065">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2066">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2066">Storage</span></span>

* <span data-ttu-id="11308-2067">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-2067">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="11308-2068">Event Grid</span><span class="sxs-lookup"><span data-stu-id="11308-2068">Eventgrid</span></span>

* <span data-ttu-id="11308-2069">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="11308-2069">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="11308-2070">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-2070">SQL</span></span>

* <span data-ttu-id="11308-2071">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2071">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="11308-2072">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="11308-2072">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="11308-2073">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2073">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-2074">Keyvault</span><span class="sxs-lookup"><span data-stu-id="11308-2074">Keyvault</span></span>

* <span data-ttu-id="11308-2075">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2075">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2076">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2076">VM</span></span>

* <span data-ttu-id="11308-2077">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2077">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="11308-2078">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="11308-2078">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="11308-2079">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2079">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="11308-2080">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2080">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="11308-2081">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2081">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="11308-2082">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2082">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2083">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2083">ACS</span></span>

* <span data-ttu-id="11308-2084">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2084">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2085">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2085">Appservice</span></span>

* <span data-ttu-id="11308-2086">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2086">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="11308-2087">Backup</span><span class="sxs-lookup"><span data-stu-id="11308-2087">Backup</span></span>

* <span data-ttu-id="11308-2088">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2088">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="11308-2089">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="11308-2089">September 11, 2017</span></span>

<span data-ttu-id="11308-2090">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="11308-2090">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="11308-2091">코어</span><span class="sxs-lookup"><span data-stu-id="11308-2091">Core</span></span>

* <span data-ttu-id="11308-2092">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2092">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="11308-2093">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2093">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2094">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2094">Acs</span></span>

* <span data-ttu-id="11308-2095">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2095">Added `acs list-locations` command</span></span>
* <span data-ttu-id="11308-2096">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="11308-2096">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2097">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2097">Appservice</span></span>

* <span data-ttu-id="11308-2098">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2098">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-2099">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-2099">CDN</span></span>

* <span data-ttu-id="11308-2100">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2100">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="11308-2101">내선 번호</span><span class="sxs-lookup"><span data-stu-id="11308-2101">Extension</span></span>

* <span data-ttu-id="11308-2102">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2102">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-2103">Keyvault</span><span class="sxs-lookup"><span data-stu-id="11308-2103">Keyvault</span></span>

* <span data-ttu-id="11308-2104">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2104">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="11308-2105">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2105">Network</span></span>

* <span data-ttu-id="11308-2106">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2106">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="11308-2107">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-2107">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="11308-2108">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2108">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="11308-2109">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2109">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="11308-2110">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2110">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2111">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2111">Resource</span></span>

* <span data-ttu-id="11308-2112">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-2112">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="11308-2113">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-2113">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="11308-2114">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="11308-2114">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="11308-2115">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="11308-2115">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="11308-2116">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-2116">SQL</span></span>

* <span data-ttu-id="11308-2117">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2117">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2118">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2118">VM</span></span>

* <span data-ttu-id="11308-2119">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2119">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="11308-2120">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="11308-2120">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="11308-2121">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2121">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="11308-2122">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2122">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="11308-2123">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2123">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="11308-2124">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="11308-2124">August 31, 2017</span></span>

<span data-ttu-id="11308-2125">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="11308-2125">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-2126">Keyvault</span><span class="sxs-lookup"><span data-stu-id="11308-2126">Keyvault</span></span>

* <span data-ttu-id="11308-2127">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2127">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="11308-2128">Sf</span><span class="sxs-lookup"><span data-stu-id="11308-2128">Sf</span></span>

* <span data-ttu-id="11308-2129">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2129">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2130">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2130">Storage</span></span>

* <span data-ttu-id="11308-2131">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2131">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="11308-2132">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="11308-2132">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="11308-2133">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="11308-2133">August 28, 2017</span></span>

<span data-ttu-id="11308-2134">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="11308-2134">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="11308-2135">CLI</span><span class="sxs-lookup"><span data-stu-id="11308-2135">CLI</span></span>

* <span data-ttu-id="11308-2136">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2136">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2137">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2137">ACS</span></span>

* <span data-ttu-id="11308-2138">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2138">Corrected preview regions</span></span>
* <span data-ttu-id="11308-2139">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2139">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="11308-2140">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="11308-2140">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2141">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2141">Appservice</span></span>

* <span data-ttu-id="11308-2142">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2142">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="11308-2143">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2143">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="11308-2144">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2144">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="11308-2145">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2145">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="11308-2146">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="11308-2146">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="11308-2147">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-2147">IoT</span></span>

* <span data-ttu-id="11308-2148">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2148">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="11308-2149">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2149">Network</span></span>

* <span data-ttu-id="11308-2150">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2150">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="11308-2151">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2151">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="11308-2152">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2152">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="11308-2153">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2153">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="11308-2154">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2154">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-2155">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-2155">Profile</span></span>

* <span data-ttu-id="11308-2156">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2156">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="11308-2157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="11308-2157">Service Fabric</span></span>

* <span data-ttu-id="11308-2158">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2158">Preview release</span></span>
* <span data-ttu-id="11308-2159">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="11308-2159">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="11308-2160">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2160">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="11308-2161">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2161">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2162">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2162">Storage</span></span>

* <span data-ttu-id="11308-2163">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2163">Enabled setting blob tier</span></span>
* <span data-ttu-id="11308-2164">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2164">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="11308-2165">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2165">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="11308-2166">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2166">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="11308-2167">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2167">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="11308-2168">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2168">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2169">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2169">VM</span></span>

* <span data-ttu-id="11308-2170">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2170">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="11308-2171">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2171">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="11308-2172">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2172">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="11308-2173">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2173">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="11308-2174">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2174">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="11308-2175">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2175">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="11308-2176">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="11308-2176">August 15, 2017</span></span>

<span data-ttu-id="11308-2177">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="11308-2177">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2178">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2178">ACS</span></span>

* <span data-ttu-id="11308-2179">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2179">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2180">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2180">Appservice</span></span>

* <span data-ttu-id="11308-2181">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2181">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="11308-2182">Event Grid</span><span class="sxs-lookup"><span data-stu-id="11308-2182">Event Grid</span></span>

* <span data-ttu-id="11308-2183">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2183">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="11308-2184">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="11308-2184">August 11, 2017</span></span>

<span data-ttu-id="11308-2185">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="11308-2185">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2186">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2186">ACS</span></span>

* <span data-ttu-id="11308-2187">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2187">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="11308-2188">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-2188">Batch</span></span>

* <span data-ttu-id="11308-2189">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2189">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="11308-2190">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2190">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="11308-2191">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2191">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="11308-2192">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2192">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="11308-2193">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2193">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="11308-2194">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2194">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="11308-2195">구성 요소</span><span class="sxs-lookup"><span data-stu-id="11308-2195">Component</span></span>

* <span data-ttu-id="11308-2196">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2196">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="11308-2197">컨테이너</span><span class="sxs-lookup"><span data-stu-id="11308-2197">Container</span></span>

* <span data-ttu-id="11308-2198">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-2198">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="11308-2199">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="11308-2199">Data Lake Store</span></span>

* <span data-ttu-id="11308-2200">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2200">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="11308-2201">Event Grid</span><span class="sxs-lookup"><span data-stu-id="11308-2201">Event Grid</span></span>

* <span data-ttu-id="11308-2202">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2202">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="11308-2203">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2203">Network</span></span>

* <span data-ttu-id="11308-2204">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-2204">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="11308-2205">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-2205">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="11308-2206">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-2206">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="11308-2207">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2207">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="11308-2208">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-2208">Profile</span></span>

* <span data-ttu-id="11308-2209">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2209">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2210">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2210">Storage</span></span>

* <span data-ttu-id="11308-2211">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2211">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2212">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2212">VM</span></span>

* <span data-ttu-id="11308-2213">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2213">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="11308-2214">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2214">Exposed `list-skus` command</span></span>
* <span data-ttu-id="11308-2215">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2215">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="11308-2216">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2216">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="11308-2217">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2217">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="11308-2218">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="11308-2218">July 28, 2017</span></span>

<span data-ttu-id="11308-2219">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="11308-2219">Version 2.0.12</span></span>

* <span data-ttu-id="11308-2220">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2220">Added container commands</span></span>
* <span data-ttu-id="11308-2221">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2221">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="11308-2222">코어</span><span class="sxs-lookup"><span data-stu-id="11308-2222">Core</span></span>

* <span data-ttu-id="11308-2223">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="11308-2223">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="11308-2224">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="11308-2224">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="11308-2225">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-2225">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="11308-2226">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="11308-2226">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="11308-2227">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="11308-2227">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="11308-2228">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="11308-2228">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="11308-2229">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="11308-2229">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="11308-2230">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="11308-2230">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="11308-2231">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="11308-2231">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="11308-2232">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="11308-2232">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="11308-2233">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="11308-2233">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="11308-2234">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="11308-2234">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="11308-2235">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2235">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="11308-2236">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2236">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="11308-2237">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2237">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="11308-2238">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="11308-2238">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="11308-2239">ACR</span><span class="sxs-lookup"><span data-stu-id="11308-2239">ACR</span></span>

* <span data-ttu-id="11308-2240">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2240">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="11308-2241">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2241">Support SKU update for managed registries</span></span>
* <span data-ttu-id="11308-2242">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2242">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="11308-2243">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2243">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="11308-2244">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2244">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="11308-2245">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2245">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2246">ACS</span></span>

* <span data-ttu-id="11308-2247">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2247">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2248">App Service</span><span class="sxs-lookup"><span data-stu-id="11308-2248">Appservice</span></span>

* <span data-ttu-id="11308-2249">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2249">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="11308-2250">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2250">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="11308-2251">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2251">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="11308-2252">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="11308-2252">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="11308-2253">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="11308-2253">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="11308-2254">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="11308-2254">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="11308-2255">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="11308-2255">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="11308-2256">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="11308-2256">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="11308-2257">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2257">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="11308-2258">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2258">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="11308-2259">Batch</span><span class="sxs-lookup"><span data-stu-id="11308-2259">Batch</span></span>

* <span data-ttu-id="11308-2260">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2260">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="11308-2261">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2261">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="11308-2262">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2262">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="11308-2263">CDN</span><span class="sxs-lookup"><span data-stu-id="11308-2263">CDN</span></span>

* <span data-ttu-id="11308-2264">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="11308-2264">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="11308-2265">클라우드</span><span class="sxs-lookup"><span data-stu-id="11308-2265">Cloud</span></span>

* <span data-ttu-id="11308-2266">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2266">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="11308-2267">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2267">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="11308-2268">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2268">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="11308-2269">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="11308-2269">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="11308-2270">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="11308-2270">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-2271">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-2271">CosmosDB</span></span>

* <span data-ttu-id="11308-2272">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2272">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="11308-2273">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2273">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="11308-2274">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="11308-2274">Data Lake Analytics</span></span>

* <span data-ttu-id="11308-2275">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2275">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="11308-2276">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2276">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="11308-2277">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2277">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="11308-2278">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="11308-2278">Data Lake Store</span></span>

* <span data-ttu-id="11308-2279">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2279">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="11308-2280">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2280">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="11308-2281">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2281">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="11308-2282">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="11308-2282">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="11308-2283">대화형</span><span class="sxs-lookup"><span data-stu-id="11308-2283">Interactive</span></span>

* <span data-ttu-id="11308-2284">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2284">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="11308-2285">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2285">Increased test coverage</span></span>
* <span data-ttu-id="11308-2286">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2286">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="11308-2287">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="11308-2287">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="11308-2288">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="11308-2288">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="11308-2289">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="11308-2289">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="11308-2290">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="11308-2290">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="11308-2291">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2291">Added `--progress` flag</span></span>
* <span data-ttu-id="11308-2292">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2292">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="11308-2293">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="11308-2293">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="11308-2294">IoT</span><span class="sxs-lookup"><span data-stu-id="11308-2294">IoT</span></span>

* <span data-ttu-id="11308-2295">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2295">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="11308-2296">(#3934)</span><span class="sxs-lookup"><span data-stu-id="11308-2296">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="11308-2297">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="11308-2297">Key vault</span></span>

* <span data-ttu-id="11308-2298">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="11308-2298">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="11308-2299">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="11308-2299">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="11308-2300">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="11308-2300">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="11308-2301">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="11308-2301">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="11308-2302">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="11308-2302">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="11308-2303">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="11308-2303">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="11308-2304">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="11308-2304">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="11308-2305">(#3307)</span><span class="sxs-lookup"><span data-stu-id="11308-2305">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="11308-2306">랩</span><span class="sxs-lookup"><span data-stu-id="11308-2306">Lab</span></span>

* <span data-ttu-id="11308-2307">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2307">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="11308-2308">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2308">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-2309">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-2309">Monitor</span></span>

* <span data-ttu-id="11308-2310">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="11308-2310">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="11308-2311">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2311">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="11308-2312">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2312">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="11308-2313">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2313">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="11308-2314">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="11308-2314">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="11308-2315">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="11308-2315">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="11308-2316">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2316">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="11308-2317">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2317">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="11308-2318">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2318">`location` no longer required</span></span>
  * <span data-ttu-id="11308-2319">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2319">Add name and ID support for target</span></span>
  * <span data-ttu-id="11308-2320">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2320">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="11308-2321">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2321">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="11308-2322">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2322">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="11308-2323">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2323">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="11308-2324">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2324">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="11308-2325">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2325">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="11308-2326">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2326">Network</span></span>

* <span data-ttu-id="11308-2327">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2327">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="11308-2328">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2328">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="11308-2329">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2329">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="11308-2330">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2330">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="11308-2331">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2331">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="11308-2332">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2332">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="11308-2333">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="11308-2333">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="11308-2334">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="11308-2334">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="11308-2335">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="11308-2335">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="11308-2336">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="11308-2336">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="11308-2337">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="11308-2337">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="11308-2338">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="11308-2338">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="11308-2339">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="11308-2339">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="11308-2340">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="11308-2340">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="11308-2341">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2341">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="11308-2342">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2342">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="11308-2343">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2343">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="11308-2344">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2344">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="11308-2345">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2345">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="11308-2346">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2346">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="11308-2347">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2347">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="11308-2348">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2348">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="11308-2349">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2349">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="11308-2350">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2350">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="11308-2351">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2351">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="11308-2352">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2352">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="11308-2353">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="11308-2353">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="11308-2354">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-2354">Profile</span></span>

* <span data-ttu-id="11308-2355">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2355">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="11308-2356">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2356">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="11308-2357">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="11308-2357">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="11308-2358">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2358">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="11308-2359">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2359">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="11308-2360">RDBMS</span><span class="sxs-lookup"><span data-stu-id="11308-2360">RDBMS</span></span>

* <span data-ttu-id="11308-2361">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="11308-2361">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="11308-2362">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="11308-2362">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="11308-2363">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="11308-2363">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="11308-2364">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="11308-2364">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2365">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2365">Resource</span></span>

* <span data-ttu-id="11308-2366">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2366">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="11308-2367">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="11308-2367">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="11308-2368">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2368">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="11308-2369">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2369">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="11308-2370">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="11308-2370">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="11308-2371">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2371">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="11308-2372">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="11308-2372">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="11308-2373">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2373">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="11308-2374">역할</span><span class="sxs-lookup"><span data-stu-id="11308-2374">Role</span></span>

* <span data-ttu-id="11308-2375">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2375">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="11308-2376">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="11308-2376">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="11308-2377">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="11308-2377">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="11308-2378">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="11308-2378">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="11308-2379">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2379">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="11308-2380">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="11308-2380">Service Fabric</span></span>
* <span data-ttu-id="11308-2381">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="11308-2381">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="11308-2382">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="11308-2382">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="11308-2383">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="11308-2383">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="11308-2384">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-2384">SQL</span></span>

* <span data-ttu-id="11308-2385">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2385">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="11308-2386">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="11308-2386">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="11308-2387">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2387">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2388">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2388">Storage</span></span>

* <span data-ttu-id="11308-2389">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="11308-2389">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="11308-2390">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="11308-2390">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="11308-2391">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="11308-2391">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="11308-2392">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2392">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="11308-2393">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="11308-2393">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="11308-2394">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="11308-2394">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2395">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2395">VM</span></span>

* <span data-ttu-id="11308-2396">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2396">Support configuring nsg</span></span>
* <span data-ttu-id="11308-2397">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2397">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="11308-2398">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="11308-2398">Support managed service identities</span></span>
* <span data-ttu-id="11308-2399">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="11308-2399">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="11308-2400">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="11308-2400">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="11308-2401">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="11308-2401">May 10, 2017</span></span>

<span data-ttu-id="11308-2402">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="11308-2402">Version 2.0.6</span></span>

* <span data-ttu-id="11308-2403">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="11308-2403">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="11308-2404">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2404">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="11308-2405">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="11308-2405">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="11308-2406">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="11308-2406">Include Cognitive Services module</span></span>
* <span data-ttu-id="11308-2407">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="11308-2407">Include Service Fabric module</span></span>
* <span data-ttu-id="11308-2408">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="11308-2408">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="11308-2409">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2409">Add support for CDN commands</span></span>
* <span data-ttu-id="11308-2410">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="11308-2410">Remove Container module</span></span>
* <span data-ttu-id="11308-2411">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="11308-2411">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="11308-2412">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="11308-2412">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="11308-2413">코어</span><span class="sxs-lookup"><span data-stu-id="11308-2413">Core</span></span>

* <span data-ttu-id="11308-2414">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="11308-2414">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="11308-2415">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="11308-2415">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="11308-2416">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="11308-2416">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="11308-2417">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="11308-2417">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="11308-2418">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="11308-2418">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="11308-2419">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="11308-2419">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="11308-2420">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="11308-2420">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="11308-2421">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="11308-2421">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="11308-2422">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="11308-2422">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="11308-2423">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="11308-2423">core: Improved performance</span></span>
* <span data-ttu-id="11308-2424">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2424">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="11308-2425">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="11308-2425">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2426">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2426">ACS</span></span>

* <span data-ttu-id="11308-2427">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2427">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="11308-2428">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="11308-2428">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="11308-2429">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="11308-2429">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="11308-2430">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="11308-2430">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2431">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-2431">AppService</span></span>

* <span data-ttu-id="11308-2432">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="11308-2432">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="11308-2433">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2433">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="11308-2434">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="11308-2434">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="11308-2435">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="11308-2435">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="11308-2436">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="11308-2436">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="11308-2437">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="11308-2437">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="11308-2438">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2438">support slot swap with preview</span></span>
* <span data-ttu-id="11308-2439">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="11308-2439">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="11308-2440">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="11308-2440">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="11308-2441">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="11308-2441">CosmosDB</span></span>

* <span data-ttu-id="11308-2442">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="11308-2442">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="11308-2443">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2443">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="11308-2444">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2444">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="11308-2445">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2445">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="11308-2446">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="11308-2446">Data Lake Analytics</span></span>

* <span data-ttu-id="11308-2447">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2447">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="11308-2448">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2448">Add support for new catalog item type: package.</span></span> <span data-ttu-id="11308-2449">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="11308-2449">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="11308-2450">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="11308-2450">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="11308-2451">테이블</span><span class="sxs-lookup"><span data-stu-id="11308-2451">Table</span></span>
  * <span data-ttu-id="11308-2452">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="11308-2452">Table valued function</span></span>
  * <span data-ttu-id="11308-2453">보기</span><span class="sxs-lookup"><span data-stu-id="11308-2453">View</span></span>
  * <span data-ttu-id="11308-2454">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="11308-2454">Table Statistics.</span></span> <span data-ttu-id="11308-2455">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="11308-2455">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="11308-2456">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="11308-2456">Data Lake Store</span></span>

* <span data-ttu-id="11308-2457">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="11308-2457">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="11308-2458">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="11308-2458">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="11308-2459">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="11308-2459">missed help for access show.</span></span> <span data-ttu-id="11308-2460">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2460">adding it.</span></span> <span data-ttu-id="11308-2461">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="11308-2461">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="11308-2462">찾기</span><span class="sxs-lookup"><span data-stu-id="11308-2462">Find</span></span>

* <span data-ttu-id="11308-2463">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="11308-2463">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="11308-2464">KeyVault</span><span class="sxs-lookup"><span data-stu-id="11308-2464">KeyVault</span></span>

* <span data-ttu-id="11308-2465">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2465">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="11308-2466">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="11308-2466">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="11308-2467">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2467">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="11308-2468">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2468">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="11308-2469">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="11308-2469">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="11308-2470">랩</span><span class="sxs-lookup"><span data-stu-id="11308-2470">Lab</span></span>

* <span data-ttu-id="11308-2471">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2471">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="11308-2472">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2472">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="11308-2473">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="11308-2473">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="11308-2474">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="11308-2474">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="11308-2475">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2475">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="11308-2476">모니터</span><span class="sxs-lookup"><span data-stu-id="11308-2476">Monitor</span></span>

* <span data-ttu-id="11308-2477">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="11308-2477">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="11308-2478">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="11308-2478">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="11308-2479">네트워크</span><span class="sxs-lookup"><span data-stu-id="11308-2479">Network</span></span>

* <span data-ttu-id="11308-2480">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2480">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="11308-2481">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2481">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="11308-2482">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2482">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="11308-2483">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2483">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="11308-2484">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2484">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="11308-2485">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2485">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="11308-2486">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2486">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="11308-2487">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2487">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="11308-2488">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2488">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="11308-2489">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2489">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="11308-2490">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="11308-2490">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="11308-2491">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2491">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="11308-2492">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2492">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="11308-2493">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2493">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="11308-2494">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="11308-2494">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="11308-2495">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2495">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="11308-2496">프로필</span><span class="sxs-lookup"><span data-stu-id="11308-2496">Profile</span></span>

* <span data-ttu-id="11308-2497">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="11308-2497">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="11308-2498">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="11308-2498">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="11308-2499">Redis</span><span class="sxs-lookup"><span data-stu-id="11308-2499">Redis</span></span>

* <span data-ttu-id="11308-2500">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2500">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="11308-2501">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="11308-2501">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="11308-2502">리소스</span><span class="sxs-lookup"><span data-stu-id="11308-2502">Resource</span></span>

* <span data-ttu-id="11308-2503">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="11308-2503">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="11308-2504">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="11308-2504">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="11308-2505">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="11308-2505">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="11308-2506">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2506">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="11308-2507">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="11308-2507">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="11308-2508">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2508">Add docs for az lock update.</span></span> <span data-ttu-id="11308-2509">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="11308-2509">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="11308-2510">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2510">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="11308-2511">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="11308-2511">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="11308-2512">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2512">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="11308-2513">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="11308-2513">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="11308-2514">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="11308-2514">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="11308-2515">역할</span><span class="sxs-lookup"><span data-stu-id="11308-2515">Role</span></span>

* <span data-ttu-id="11308-2516">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="11308-2516">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="11308-2517">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="11308-2517">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="11308-2518">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="11308-2518">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="11308-2519">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="11308-2519">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="11308-2520">SQL</span><span class="sxs-lookup"><span data-stu-id="11308-2520">SQL</span></span>

* <span data-ttu-id="11308-2521">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="11308-2521">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="11308-2522">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="11308-2522">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="11308-2523">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2523">Storage</span></span>

* <span data-ttu-id="11308-2524">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="11308-2524">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="11308-2525">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2525">Add support for incremental blob copy</span></span>
* <span data-ttu-id="11308-2526">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2526">Add support for large block blob upload</span></span>
* <span data-ttu-id="11308-2527">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="11308-2527">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2528">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2528">VM</span></span>

* <span data-ttu-id="11308-2529">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="11308-2529">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="11308-2530">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="11308-2530">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="11308-2531">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="11308-2531">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="11308-2532">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="11308-2532">az vm/vmss disk</span></span>
  3. <span data-ttu-id="11308-2533">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2533">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="11308-2534">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="11308-2534">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="11308-2535">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="11308-2535">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="11308-2536">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="11308-2536">April 3, 2017</span></span>

<span data-ttu-id="11308-2537">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="11308-2537">Version 2.0.2</span></span>

<span data-ttu-id="11308-2538">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2538">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="11308-2539">코어</span><span class="sxs-lookup"><span data-stu-id="11308-2539">Core</span></span>

* <span data-ttu-id="11308-2540">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="11308-2540">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="11308-2541">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="11308-2541">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="11308-2542">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="11308-2542">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="11308-2543">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="11308-2543">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="11308-2544">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="11308-2544">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="11308-2545">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="11308-2545">Add prompting for missing template parameters.</span></span> <span data-ttu-id="11308-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="11308-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="11308-2547">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2547">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="11308-2548">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="11308-2548">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="11308-2549">ACS</span><span class="sxs-lookup"><span data-stu-id="11308-2549">ACS</span></span>

* <span data-ttu-id="11308-2550">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="11308-2550">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="11308-2551">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="11308-2551">Add support for ssh key password prompting.</span></span> <span data-ttu-id="11308-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="11308-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="11308-2553">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="11308-2553">Add support for windows clusters.</span></span> <span data-ttu-id="11308-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="11308-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="11308-2555">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="11308-2555">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="11308-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="11308-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="11308-2557">AppService</span><span class="sxs-lookup"><span data-stu-id="11308-2557">AppService</span></span>

* <span data-ttu-id="11308-2558">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="11308-2558">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="11308-2559">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="11308-2559">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="11308-2560">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="11308-2560">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="11308-2561">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="11308-2561">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="11308-2562">DataLake</span><span class="sxs-lookup"><span data-stu-id="11308-2562">DataLake</span></span>

* <span data-ttu-id="11308-2563">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2563">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="11308-2564">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="11308-2564">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="11308-2565">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="11308-2565">DocuemntDB</span></span>

* <span data-ttu-id="11308-2566">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="11308-2566">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="11308-2567">VM</span><span class="sxs-lookup"><span data-stu-id="11308-2567">VM</span></span>

* <span data-ttu-id="11308-2568">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="11308-2568">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="11308-2569">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="11308-2569">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="11308-2570">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="11308-2570">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="11308-2571">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="11308-2571">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="11308-2572">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="11308-2572">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="11308-2573">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="11308-2573">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="11308-2574">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="11308-2574">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="11308-2575">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="11308-2575">February 27, 2017</span></span>

<span data-ttu-id="11308-2576">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="11308-2576">Version 2.0.0</span></span>

<span data-ttu-id="11308-2577">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2577">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="11308-2578">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="11308-2578">Container Service (acs)</span></span>
- <span data-ttu-id="11308-2579">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="11308-2579">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="11308-2580">네트워킹</span><span class="sxs-lookup"><span data-stu-id="11308-2580">Networking</span></span>
- <span data-ttu-id="11308-2581">Storage</span><span class="sxs-lookup"><span data-stu-id="11308-2581">Storage</span></span>

<span data-ttu-id="11308-2582">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2582">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="11308-2583">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2583">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="11308-2584">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2584">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="11308-2585">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2585">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="11308-2586">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="11308-2586">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="11308-2587">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="11308-2587">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="11308-2588">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="11308-2588">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="11308-2589">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="11308-2589">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="11308-2590">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="11308-2590">Provide feedback from the command line with the `az feedback` command</span></span>


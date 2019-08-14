---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/13/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d315046287a552e89112fa415e1219f9a97d4944
ms.sourcegitcommit: b00555c528697c0a6419cf23380e48c8705026db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2019
ms.locfileid: "68974272"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="24041-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="24041-103">Azure CLI release notes</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="24041-104">2019년 8월 13일</span><span class="sxs-lookup"><span data-stu-id="24041-104">August 13, 2019</span></span>

<span data-ttu-id="24041-105">버전 2.0.71</span><span class="sxs-lookup"><span data-stu-id="24041-105">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-106">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-106">AppService</span></span>

* <span data-ttu-id="24041-107">슬롯에 대해 `webapp webjob continuous` 명령이 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-107">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-108">BotService</span><span class="sxs-lookup"><span data-stu-id="24041-108">BotService</span></span>

* <span data-ttu-id="24041-109">[호환성이 손상되는 변경] v3 SDK 봇 만들기에 대한 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-109">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="24041-110">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24041-110">CognitiveServices</span></span>

* <span data-ttu-id="24041-111">`cognitiveservices account network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-111">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="24041-112">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="24041-112">Cosmos DB</span></span>

* <span data-ttu-id="24041-113">여러 쓰기 위치 업데이트 시의 경고가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-113">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="24041-114">CosmosDB SQL, MongoDB, Cassandra, Gremlin 및 Table 리소스 및 리소스 처리량에 대한 CRUD 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-114">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-115">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-115">HDInsight</span></span>

<span data-ttu-id="24041-116">이 릴리스에는 호환성이 손상되는 변경이 많이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-116">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="24041-117">[호환성이 손상되는 변경] `hdinsight create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-117">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="24041-118">이름이 `--storage-default-container`에서 `--storage-container`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-118">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="24041-119">이름이 `--storage-default-filesystem`에서 `--storage-filesystem`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-119">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="24041-120">[호환성이 손상되는 변경] `application create`의 `--name` 인수에서 클러스터 이름 대신 애플리케이션 이름을 나타내도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-120">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="24041-121">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 `application create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-121">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="24041-122">[호환성이 손상되는 변경] `application create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-122">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="24041-123">이름이 `--application-type`에서 `--type`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-123">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="24041-124">이름이 `--marketplace-identifier`에서 `--marketplace-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-124">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="24041-125">이름이 `--https-endpoint-access-mode`에서 `--access-mode`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-125">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="24041-126">이름이 `--https-endpoint-destination-port`에서 `--destination-port`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-126">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="24041-127">[호환성이 손상되는 변경] `application create`에 대한 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-127">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="24041-128">[호환성이 손상되는 변경] `hdinsight resize`에 대한 이름이 `--target-instance-count`에서 `--workernode-count`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-128">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="24041-129">[호환성이 손상되는 변경] `hdinsight script-action` 그룹의 모든 명령에서 `--name` 매개 변수를 스크립트 작업 이름으로 사용하도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="24041-129">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="24041-130">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 모든 `hdinsight script-action` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-130">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="24041-131">[호환성이 손상되는 변경] 모든 `hdinsight script-action` 명령에 대한 이름이 `--script-execution-id`에서 `--execution-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-131">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="24041-132">[호환성이 손상되는 변경] `hdinsight script-action show`에서 `hdinsight script-action show-execution-details`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-132">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="24041-133">[호환성이 손상되는 변경] `hdinsight script-action execute --roles`의 매개 변수에서 쉼표로 구분하는 대신 공백으로 구분하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-133">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="24041-134">[호환성이 손상되는 변경] `hdinsight script-action list`의 `--persisted` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-134">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="24041-135">`hdinsight create --cluster-configurations` 매개 변수에서 로컬 JSON 파일 또는 JSON 문자열에 대한 경로를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-135">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="24041-136">명령 `hdinsight script-action list-execution-history` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-136">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="24041-137">`hdinsight monitor enable --workspace`에서 Log Analytics 작업 영역 ID 또는 작업 영역 이름을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-137">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="24041-138">작업 영역 ID가 매개 변수로 제공되는 경우 필요한 `hdinsight monitor enable --primary-key` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-138">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="24041-139">도움말 메시지에 대한 추가 예제 및 업데이트된 설명이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-139">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-140">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-140">Interactive</span></span>

* <span data-ttu-id="24041-141">로드 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-141">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="24041-142">kubernetes</span><span class="sxs-lookup"><span data-stu-id="24041-142">Kubernetes</span></span>

* <span data-ttu-id="24041-143">대시보드 컨테이너 포트에서 `https`를 사용하는 경우 `https`를 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-143">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="24041-144">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-144">Network</span></span>

* <span data-ttu-id="24041-145">`--yes` 인수가 `network dns record-set cname delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-145">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-146">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-146">Profile</span></span>

* <span data-ttu-id="24041-147">리소스 액세스 토큰을 가져오기 위해 `--resource-type` 인수가 `account get-access-token`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-147">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="24041-148">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24041-148">ServiceFabric</span></span>

* <span data-ttu-id="24041-149">sf 클러스터를 만드는 데 지원되는 모든 os 버전이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-149">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="24041-150">기본 인증서 유효성 검사 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-150">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="24041-151">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-151">Storage</span></span>

* <span data-ttu-id="24041-152">명령 `storage copy` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-152">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="24041-153">2019년 7월 30일</span><span class="sxs-lookup"><span data-stu-id="24041-153">July 30, 2019</span></span>

<span data-ttu-id="24041-154">버전 2.0.70</span><span class="sxs-lookup"><span data-stu-id="24041-154">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="24041-155">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-155">ACR</span></span>

* <span data-ttu-id="24041-156">#9952 문제(`acr pack build` 명령의 회귀)가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-156">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="24041-157">`acr pack build`의 기본 작성기 이미지 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-157">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-158">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-158">Appservice</span></span>

* <span data-ttu-id="24041-159">리소스를 찾을 수 없는 경우 메시지를 표시 하도록 `webapp config ssl`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-159">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="24041-160">`functionapp create`에서 `Standard_RAGRS` 스토리지 계정 유형을 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-160">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="24041-161">이전 버전의 python을 사용하여 실행할 경우 `webapp up`이(가) 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-161">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="24041-162">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-162">Network</span></span>

* <span data-ttu-id="24041-163">`network nic ip-config add`에서 잘못된 매개 변수 `--ids` 제거됨(#9861 수정)</span><span class="sxs-lookup"><span data-stu-id="24041-163">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="24041-164">#9604 수정.</span><span class="sxs-lookup"><span data-stu-id="24041-164">Fixes #9604.</span></span> <span data-ttu-id="24041-165">사용자가 신뢰할 수 있는 루트 인증서를 연결할 수 있도록 `network application-gateway http-settings [create|update]`에 `--root-certs` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-165">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="24041-166">`network dns record-set ns create`(#9965)에 대해 인수 `--subscription`을 수정</span><span class="sxs-lookup"><span data-stu-id="24041-166">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="24041-167">RBAC</span><span class="sxs-lookup"><span data-stu-id="24041-167">RBAC</span></span>

* <span data-ttu-id="24041-168">`user update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-168">Added `user update` command</span></span>
* <span data-ttu-id="24041-169">[사용 되지 않음] 사용자 관련 명령 중 `--upn-or-object-id`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-169">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="24041-170">대체 인수 `--id` 사용</span><span class="sxs-lookup"><span data-stu-id="24041-170">Use replacement argument `--id`</span></span>
* <span data-ttu-id="24041-171">사용자 관련 명령에 `--id` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-171">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="24041-172">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-172">SQL</span></span>

* <span data-ttu-id="24041-173">관리형 인스턴스 키 및 TDE 보호기에 대한 관리 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-173">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="24041-174">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-174">Storage</span></span>

* <span data-ttu-id="24041-175">`storage remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-175">Added `storage remove` command</span></span>
* <span data-ttu-id="24041-176">`storage blob update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-176">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-177">VM</span><span class="sxs-lookup"><span data-stu-id="24041-177">VM</span></span>

* <span data-ttu-id="24041-178">새로운 API 버전을 사용하여 영역 세부 정보를 출력하도록 `list-skus`를 변경</span><span class="sxs-lookup"><span data-stu-id="24041-178">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="24041-179">`vmss create`에 대한 `--single-placement-group`의 기본값을 `false`로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-179">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="24041-180">`[snapshot|disk] create`에 대한 ZRS 스토리지 SKU를 선택하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-180">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="24041-181">전용 호스트를 지원하는 새로운 명령 그룹 `vm host`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-181">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="24041-182">VM 전용 호스트를 설정하기 위해 `vm create`에 매개 변수 `--host` 및 `--host-group` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-182">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="24041-183">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="24041-183">July 16, 2019</span></span>

<span data-ttu-id="24041-184">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="24041-184">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-185">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-185">Appservice</span></span>

* <span data-ttu-id="24041-186">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-186">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="24041-187">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-187">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="24041-188">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="24041-188">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="24041-189">코어</span><span class="sxs-lookup"><span data-stu-id="24041-189">Core</span></span>

* <span data-ttu-id="24041-190">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-190">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="24041-191">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-191">Batch</span></span>

* <span data-ttu-id="24041-192">[호환성이 손상되는 변경] `batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="24041-192">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="24041-193">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-193">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="24041-194">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-194">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="24041-195">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-195">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="24041-196">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="24041-196">Eventhubs</span></span>

* <span data-ttu-id="24041-197">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-197">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-198">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-198">RDBMS</span></span>

* <span data-ttu-id="24041-199">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-199">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="24041-200">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="24041-200">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="24041-201">릴레이</span><span class="sxs-lookup"><span data-stu-id="24041-201">Relay</span></span>

* <span data-ttu-id="24041-202">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-202">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="24041-203">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-203">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="24041-204">Servicebus</span><span class="sxs-lookup"><span data-stu-id="24041-204">Servicebus</span></span>

* <span data-ttu-id="24041-205">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-205">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="24041-206">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-206">Storage</span></span>

* <span data-ttu-id="24041-207">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="24041-207">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="24041-208">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="24041-208">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="24041-209">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="24041-209">July 2, 2019</span></span>

<span data-ttu-id="24041-210">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="24041-210">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="24041-211">코어</span><span class="sxs-lookup"><span data-stu-id="24041-211">Core</span></span>

* <span data-ttu-id="24041-212">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-212">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="24041-213">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-213">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="24041-214">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-214">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="24041-215">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-215">ACR</span></span>

* <span data-ttu-id="24041-216">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-216">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-217">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-217">Appservice</span></span>

* <span data-ttu-id="24041-218">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-218">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="24041-219">[호환성이 손상되는 변경] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="24041-219">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="24041-220">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="24041-220">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="24041-221">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-221">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="24041-222">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="24041-222">Cosmos DB</span></span>

* <span data-ttu-id="24041-223">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-223">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="24041-224">DLS</span><span class="sxs-lookup"><span data-stu-id="24041-224">DLS</span></span>

* <span data-ttu-id="24041-225">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="24041-225">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="24041-226">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="24041-226">Feedback</span></span>

* <span data-ttu-id="24041-227">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-227">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-228">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-228">HDInsight</span></span>

* <span data-ttu-id="24041-229">[호환성이 손상되는 변경] `oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-229">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="24041-230">[호환성이 손상되는 변경] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-230">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="24041-231">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="24041-231">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="24041-232">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-232">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="24041-233">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="24041-233">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="24041-234">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="24041-234">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="24041-235">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-235">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="24041-236">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-236">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="24041-237">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-237">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="24041-238">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="24041-238">Managed Services</span></span>

* <span data-ttu-id="24041-239">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="24041-239">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="24041-240">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-240">Profile</span></span>
* <span data-ttu-id="24041-241">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-241">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="24041-242">RBAC</span><span class="sxs-lookup"><span data-stu-id="24041-242">RBAC</span></span>

* <span data-ttu-id="24041-243">[호환성이 손상되는 변경] `create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-243">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="24041-244">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-244">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="24041-245">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="24041-245">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="24041-246">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-246">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-247">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-247">RDBMS</span></span>

* <span data-ttu-id="24041-248">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-248">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="24041-249">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-249">SQL</span></span>

* <span data-ttu-id="24041-250">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="24041-250">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-251">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-251">Storage</span></span>

* <span data-ttu-id="24041-252">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="24041-252">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="24041-253">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="24041-253">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="24041-254">VM</span><span class="sxs-lookup"><span data-stu-id="24041-254">VM</span></span>

* <span data-ttu-id="24041-255">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-255">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="24041-256">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="24041-256">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="24041-257">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="24041-257">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="24041-258">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-258">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="24041-259">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="24041-259">June 18, 2019</span></span>

<span data-ttu-id="24041-260">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="24041-260">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="24041-261">코어</span><span class="sxs-lookup"><span data-stu-id="24041-261">Core</span></span>

<span data-ttu-id="24041-262">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-262">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="24041-263">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-263">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="24041-264">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-264">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="24041-265">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-265">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="24041-266">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-266">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="24041-267">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-267">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="24041-268">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-268">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="24041-269">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-269">ACR</span></span>
* <span data-ttu-id="24041-270">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-270">Added 'acr check-health' command</span></span>
* <span data-ttu-id="24041-271">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="24041-271">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="24041-272">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-272">ACS</span></span>
* <span data-ttu-id="24041-273">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="24041-273">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="24041-274">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-274">AMS</span></span>
* <span data-ttu-id="24041-275">[호환성이 손상되는 변경] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-275">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-276">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-276">AppService</span></span>
* <span data-ttu-id="24041-277">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="24041-277">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="24041-278">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-278">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="24041-279">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-279">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="24041-280">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-280">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="24041-281">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-281">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="24041-282">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-282">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="24041-283">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-283">Batch</span></span>
* <span data-ttu-id="24041-284">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-284">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-285">BatchAI</span><span class="sxs-lookup"><span data-stu-id="24041-285">BatchAI</span></span>
* <span data-ttu-id="24041-286">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="24041-286">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-287">BotService</span><span class="sxs-lookup"><span data-stu-id="24041-287">BotService</span></span>
* <span data-ttu-id="24041-288">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="24041-288">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-289">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-289">CosmosDB</span></span>
* <span data-ttu-id="24041-290">[사용 되지 않음] `cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-290">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="24041-291">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="24041-291">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="24041-292">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-292">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="24041-293">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-293">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="24041-294">EventGrid</span><span class="sxs-lookup"><span data-stu-id="24041-294">EventGrid</span></span>
* <span data-ttu-id="24041-295">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-295">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="24041-296">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-296">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="24041-297">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-297">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="24041-298">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="24041-298">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="24041-299">[호환성이 손상되는 변경] `eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="24041-299">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-300">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-300">HDInsight</span></span>
* <span data-ttu-id="24041-301">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-301">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="24041-302">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-302">IoT</span></span>
* <span data-ttu-id="24041-303">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-303">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="24041-304">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-304">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="24041-305">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-305">Network</span></span>
* <span data-ttu-id="24041-306">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-306">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="24041-307">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-307">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="24041-308">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-308">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="24041-309">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-309">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="24041-310">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-310">Resource</span></span>
* <span data-ttu-id="24041-311">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-311">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="24041-312">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="24041-312">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="24041-313">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24041-313">ServiceBus</span></span>
* <span data-ttu-id="24041-314">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-314">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="24041-315">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-315">SQL</span></span>
* <span data-ttu-id="24041-316">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-316">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="24041-317">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-317">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="24041-318">SQLVm</span><span class="sxs-lookup"><span data-stu-id="24041-318">SQLVm</span></span>
* <span data-ttu-id="24041-319">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-319">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="24041-320">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-320">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="24041-321">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-321">Storage</span></span>
* <span data-ttu-id="24041-322">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-322">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="24041-323">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="24041-323">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="24041-324">VM</span><span class="sxs-lookup"><span data-stu-id="24041-324">VM</span></span>
* <span data-ttu-id="24041-325">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-325">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="24041-326">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="24041-326">June 4, 2019</span></span>

<span data-ttu-id="24041-327">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="24041-327">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="24041-328">코어</span><span class="sxs-lookup"><span data-stu-id="24041-328">Core</span></span>
* <span data-ttu-id="24041-329">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-329">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="24041-330">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-330">ACR</span></span>
* <span data-ttu-id="24041-331">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-331">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="24041-332">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-332">ACS</span></span>
* <span data-ttu-id="24041-333">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="24041-333">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="24041-334">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="24041-334">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="24041-335">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-335">Batch</span></span>
* <span data-ttu-id="24041-336">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-336">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="24041-337">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-337">IoT</span></span>
* <span data-ttu-id="24041-338">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-338">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="24041-339">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-339">Network</span></span>
* <span data-ttu-id="24041-340">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-340">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="24041-341">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-341">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="24041-342">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-342">Resource</span></span>
* <span data-ttu-id="24041-343">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-343">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="24041-344">역할</span><span class="sxs-lookup"><span data-stu-id="24041-344">Role</span></span>
* <span data-ttu-id="24041-345">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-345">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="24041-346">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="24041-346">Compute</span></span>
* <span data-ttu-id="24041-347">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-347">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="24041-348">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="24041-348">May 21, 2019</span></span>

<span data-ttu-id="24041-349">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="24041-349">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="24041-350">코어</span><span class="sxs-lookup"><span data-stu-id="24041-350">Core</span></span>
* <span data-ttu-id="24041-351">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-351">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="24041-352">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-352">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="24041-353">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-353">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="24041-354">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-354">ACR</span></span>
* <span data-ttu-id="24041-355">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-355">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="24041-356">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-356">ACS</span></span>
* <span data-ttu-id="24041-357">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-357">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-358">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-358">AppService</span></span>
* <span data-ttu-id="24041-359">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-359">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="24041-360">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-360">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="24041-361">[호환성이 손상되는 변경] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-361">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="24041-362">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-362">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="24041-363">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-363">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="24041-364">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-364">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="24041-365">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-365">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-366">BotService</span><span class="sxs-lookup"><span data-stu-id="24041-366">BotService</span></span>
* <span data-ttu-id="24041-367">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-367">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="24041-368">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-368">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-369">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-369">Consumption</span></span>
* <span data-ttu-id="24041-370">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-370">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="24041-371">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-371">IoT</span></span>
* <span data-ttu-id="24041-372">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-372">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="24041-373">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-373">Network</span></span>
* [호환성이 손상되는 변경]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="24041-375">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-375">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="24041-376">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-376">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-377">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-377">RDBMS</span></span>
* <span data-ttu-id="24041-378">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-378">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="24041-379">RBAC</span><span class="sxs-lookup"><span data-stu-id="24041-379">RBAC</span></span>
* <span data-ttu-id="24041-380">`role assignment`에 관리 그룹 범위가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-380">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-381">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-381">Storage</span></span>
* <span data-ttu-id="24041-382">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-382">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="24041-383">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="24041-383">Compute</span></span>
* <span data-ttu-id="24041-384">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-384">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="24041-385">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-385">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="24041-386">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="24041-386">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="24041-387">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-387">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="24041-388">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="24041-388">May 6, 2019</span></span>

<span data-ttu-id="24041-389">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="24041-389">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="24041-390">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-390">ACS</span></span>
* <span data-ttu-id="24041-391">[호환성이 손상되는 변경] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-391">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="24041-392">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-392">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="24041-393">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-393">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="24041-394">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-394">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-395">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-395">Appservice</span></span>
* <span data-ttu-id="24041-396">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-396">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="24041-397">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-397">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="24041-398">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-398">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="24041-399">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-399">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="24041-400">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-400">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="24041-401">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-401">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="24041-402">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-402">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="24041-403">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-403">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="24041-404">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-404">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="24041-405">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-405">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="24041-406">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-406">Batch</span></span>
* <span data-ttu-id="24041-407">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-407">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-408">Botservice</span><span class="sxs-lookup"><span data-stu-id="24041-408">Botservice</span></span>
* <span data-ttu-id="24041-409">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="24041-409">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="24041-410">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-410">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="24041-411">[호환성이 손상되는 변경] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-411">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="24041-412">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="24041-412">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="24041-413">[호환성이 손상되는 변경] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-413">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="24041-414">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="24041-414">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="24041-415">[호환성이 손상되는 변경] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-415">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="24041-416">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-416">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="24041-417">[호환성이 손상되는 변경] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-417">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="24041-418">[호환성이 손상되는 변경] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-418">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="24041-419">[호환성이 손상되는 변경] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-419">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="24041-420">[호환성이 손상되는 변경] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-420">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="24041-421">[호환성이 손상되는 변경] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-421">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="24041-422">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="24041-422">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="24041-423">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="24041-423">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="24041-424">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-424">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="24041-425">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-425">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="24041-426">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-426">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="24041-427">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-427">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="24041-428">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-428">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="24041-429">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-429">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="24041-430">구성</span><span class="sxs-lookup"><span data-stu-id="24041-430">Configure</span></span>
* <span data-ttu-id="24041-431">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-431">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="24041-432">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="24041-432">Eventhubs</span></span>
* <span data-ttu-id="24041-433">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-433">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="24041-434">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-434">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="24041-435">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-435">Network</span></span>
* <span data-ttu-id="24041-436">[호환성이 손상되는 변경] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="24041-436">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="24041-437">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="24041-437">Policy Insights</span></span>
* <span data-ttu-id="24041-438">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-438">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="24041-439">역할</span><span class="sxs-lookup"><span data-stu-id="24041-439">Role</span></span>
* <span data-ttu-id="24041-440">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-440">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="24041-441">Service Bus</span><span class="sxs-lookup"><span data-stu-id="24041-441">Service Bus</span></span>
* <span data-ttu-id="24041-442">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-442">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="24041-443">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-443">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="24041-444">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-444">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="24041-445">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-445">SQL</span></span>
* <span data-ttu-id="24041-446">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-446">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="24041-447">VM</span><span class="sxs-lookup"><span data-stu-id="24041-447">VM</span></span>
* <span data-ttu-id="24041-448">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-448">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="24041-449">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-449">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="24041-450">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-450">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="24041-451">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-451">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="24041-452">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-452">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="24041-453">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-453">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="24041-454">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="24041-454">April 23, 2019</span></span>

<span data-ttu-id="24041-455">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="24041-455">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="24041-456">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-456">ACS</span></span>
* <span data-ttu-id="24041-457">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-457">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="24041-458">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="24041-458">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="24041-459">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-459">AMS</span></span>
* <span data-ttu-id="24041-460">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-460">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-461">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-461">AppService</span></span>
* <span data-ttu-id="24041-462">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-462">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="24041-463">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-463">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="24041-464">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-464">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="24041-465">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-465">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="24041-466">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-466">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="24041-467">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="24041-467">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="24041-468">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-468">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="24041-469">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="24041-469">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="24041-470">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-470">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="24041-471">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="24041-471">Deployment Manager</span></span>
* <span data-ttu-id="24041-472">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="24041-472">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="24041-473">랩</span><span class="sxs-lookup"><span data-stu-id="24041-473">Lab</span></span>
* <span data-ttu-id="24041-474">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-474">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="24041-475">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-475">Network</span></span>
* <span data-ttu-id="24041-476">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-476">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="24041-477">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-477">Resource</span></span>
* <span data-ttu-id="24041-478">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="24041-478">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="24041-479">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="24041-479">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="24041-480">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-480">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="24041-481">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-481">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="24041-482">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-482">SQL</span></span>
* <span data-ttu-id="24041-483">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-483">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="24041-484">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-484">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="24041-485">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-485">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="24041-486">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-486">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-487">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-487">Storage</span></span>
* <span data-ttu-id="24041-488">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-488">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-489">VM</span><span class="sxs-lookup"><span data-stu-id="24041-489">VM</span></span>
* <span data-ttu-id="24041-490">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-490">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="24041-491">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-491">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="24041-492">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-492">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="24041-493">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="24041-493">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="24041-494">코어</span><span class="sxs-lookup"><span data-stu-id="24041-494">Core</span></span>
* <span data-ttu-id="24041-495">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-495">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="24041-496">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-496">ACR</span></span>
* <span data-ttu-id="24041-497">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-497">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="24041-498">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-498">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="24041-501">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-501">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="24041-502">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-502">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-503">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-503">AppService</span></span>
* <span data-ttu-id="24041-504">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-504">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="24041-505">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-505">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="24041-506">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="24041-506">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="24041-507">[호환성이 손상되는 변경] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="24041-507">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="24041-508">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-508">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="24041-509">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-509">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="24041-510">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-510">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-511">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-511">CDN</span></span>
* <span data-ttu-id="24041-512">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-512">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="24041-513">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="24041-513">Feedback</span></span>
* <span data-ttu-id="24041-514">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-514">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="24041-515">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-515">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="24041-516">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-516">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-517">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-517">Monitor</span></span>
* <span data-ttu-id="24041-518">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-518">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="24041-519">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-519">Network</span></span>
* <span data-ttu-id="24041-520">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-520">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="24041-521">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-521">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="24041-522">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-522">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="24041-523">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="24041-523">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="24041-524">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="24041-524">PrivateDNS</span></span>
* <span data-ttu-id="24041-525">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-525">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="24041-526">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-526">Resource</span></span>
* <span data-ttu-id="24041-527">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-527">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="24041-528">역할</span><span class="sxs-lookup"><span data-stu-id="24041-528">Role</span></span>
* <span data-ttu-id="24041-529">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-529">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="24041-530">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-530">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="24041-531">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-531">SQL</span></span>
* <span data-ttu-id="24041-532">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-532">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="24041-533">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-533">Storage</span></span>
* <span data-ttu-id="24041-534">[호환성이 손상되는 변경] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="24041-534">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="24041-535">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-535">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="24041-536">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-536">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="24041-537">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-537">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="24041-538">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="24041-538">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="24041-539">코어</span><span class="sxs-lookup"><span data-stu-id="24041-539">Core</span></span>
* <span data-ttu-id="24041-540">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-540">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="24041-541">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="24041-541">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="24041-542">클라우드</span><span class="sxs-lookup"><span data-stu-id="24041-542">Cloud</span></span>
* <span data-ttu-id="24041-543">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-543">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="24041-544">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-544">ACR</span></span>
* <span data-ttu-id="24041-545">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="24041-545">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="24041-546">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-546">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="24041-547">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-547">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="24041-548">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-548">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-549">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-549">AppService</span></span>
* <span data-ttu-id="24041-550">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-550">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="24041-551">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-551">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="24041-552">BOT Service</span><span class="sxs-lookup"><span data-stu-id="24041-552">BOT Service</span></span>
* <span data-ttu-id="24041-553">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-553">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="24041-554">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-554">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="24041-555">[호환성이 손상되는 변경] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-555">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="24041-556">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-556">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-557">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-557">CDN</span></span>
* <span data-ttu-id="24041-558">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-558">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="24041-560">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-560">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="24041-561">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-561">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-562">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="24041-562">Cosmosdb</span></span>
* <span data-ttu-id="24041-563">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-563">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="24041-564">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-564">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-565">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-565">Interactive</span></span>
* <span data-ttu-id="24041-566">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-566">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-567">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-567">Monitor</span></span>
* <span data-ttu-id="24041-568">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-568">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="24041-569">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-569">Network</span></span>
* <span data-ttu-id="24041-570">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-570">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-571">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-571">Profile</span></span>
* <span data-ttu-id="24041-572">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-572">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="24041-573">Postgres</span><span class="sxs-lookup"><span data-stu-id="24041-573">Postgres</span></span> 
* <span data-ttu-id="24041-574">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-574">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="24041-575">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-575">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="24041-576">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-576">Resource</span></span>
* <span data-ttu-id="24041-577">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-577">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="24041-578">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-578">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="24041-579">그래프</span><span class="sxs-lookup"><span data-stu-id="24041-579">Graph</span></span>
* <span data-ttu-id="24041-580">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-580">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="24041-581">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-581">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="24041-582">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-582">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="24041-583">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-583">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="24041-584">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-584">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="24041-585">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-585">storage</span></span>
* <span data-ttu-id="24041-586">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-586">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="24041-587">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-587">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="24041-588">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-588">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="24041-589">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-589">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="24041-590">VM</span><span class="sxs-lookup"><span data-stu-id="24041-590">VM</span></span>
* <span data-ttu-id="24041-591">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-591">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="24041-592">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="24041-592">March 12, 2019</span></span>

<span data-ttu-id="24041-593">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="24041-593">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="24041-594">코어</span><span class="sxs-lookup"><span data-stu-id="24041-594">Core</span></span>

* <span data-ttu-id="24041-595">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="24041-595">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="24041-596">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-596">ACR</span></span>

* <span data-ttu-id="24041-597">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="24041-597">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="24041-598">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-598">ACS</span></span>

* <span data-ttu-id="24041-599">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-599">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="24041-600">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-600">AppService</span></span>

* <span data-ttu-id="24041-601">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-601">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="24041-602">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="24041-602">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="24041-603">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-603">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="24041-604">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="24041-604">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-605">Botservice</span><span class="sxs-lookup"><span data-stu-id="24041-605">Botservice</span></span>

* <span data-ttu-id="24041-606">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-606">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="24041-607">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-607">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="24041-608">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="24041-608">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="24041-609">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-609">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="24041-610">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-610">Container</span></span>

* <span data-ttu-id="24041-611">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-611">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="24041-612">EventHub</span><span class="sxs-lookup"><span data-stu-id="24041-612">EventHub</span></span>

* <span data-ttu-id="24041-613">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-613">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="24041-614">찾기</span><span class="sxs-lookup"><span data-stu-id="24041-614">Find</span></span>

* <span data-ttu-id="24041-615">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-615">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-616">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-616">HDInsight</span></span>

* <span data-ttu-id="24041-617">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-617">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="24041-618">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-618">Network</span></span>

* <span data-ttu-id="24041-619">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-619">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-620">Rdbms</span><span class="sxs-lookup"><span data-stu-id="24041-620">Rdbms</span></span>

* <span data-ttu-id="24041-621">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="24041-621">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="24041-622">역할</span><span class="sxs-lookup"><span data-stu-id="24041-622">Role</span></span>

* <span data-ttu-id="24041-623">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-623">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="24041-624">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-624">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="24041-625">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="24041-625">Service Fabric</span></span>

* <span data-ttu-id="24041-626">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-626">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="24041-627">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="24041-627">February 26, 2019</span></span>

<span data-ttu-id="24041-628">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="24041-628">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="24041-629">코어</span><span class="sxs-lookup"><span data-stu-id="24041-629">Core</span></span>

* <span data-ttu-id="24041-630">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-630">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="24041-631">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-631">ACR</span></span>

* <span data-ttu-id="24041-632">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-632">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="24041-633">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="24041-633">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="24041-634">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-634">ACS</span></span>

* <span data-ttu-id="24041-635">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-635">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-636">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-636">AppService</span></span>

* <span data-ttu-id="24041-637">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-637">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="24041-638">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-638">Batch</span></span>
* <span data-ttu-id="24041-639">[호환성이 손상되는 변경] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-639">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="24041-640">[호환성이 손상되는 변경] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-640">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="24041-641">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-641">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="24041-642">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-642">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="24041-643">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-643">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="24041-644">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-644">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-645">CosmosDB</span></span>

* <span data-ttu-id="24041-646">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-646">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="24041-647">Kusto</span><span class="sxs-lookup"><span data-stu-id="24041-647">Kusto</span></span>

* <span data-ttu-id="24041-648">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-648">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="24041-649">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-649">Network</span></span>

* <span data-ttu-id="24041-650">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-650">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="24041-651">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-651">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="24041-652">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-652">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="24041-653">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="24041-653">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="24041-654">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-654">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="24041-655">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-655">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="24041-656">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-656">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="24041-657">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-657">Resource</span></span>

* <span data-ttu-id="24041-658">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-658">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="24041-659">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-659">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="24041-660">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-660">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="24041-661">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="24041-661">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="24041-662">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-662">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="24041-663">역할</span><span class="sxs-lookup"><span data-stu-id="24041-663">Role</span></span>

* <span data-ttu-id="24041-664">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-664">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-665">VM</span><span class="sxs-lookup"><span data-stu-id="24041-665">VM</span></span>

* <span data-ttu-id="24041-666">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-666">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="24041-667">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="24041-667">February 12, 2019</span></span>

<span data-ttu-id="24041-668">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="24041-668">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="24041-669">코어</span><span class="sxs-lookup"><span data-stu-id="24041-669">Core</span></span>

* <span data-ttu-id="24041-670">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-670">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="24041-671">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-671">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="24041-672">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-672">ACR</span></span>
* <span data-ttu-id="24041-673">[호환성이 손상되는 변경] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-673">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="24041-674">[호환성이 손상되는 변경] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-674">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="24041-675">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-675">ACS</span></span>
* <span data-ttu-id="24041-676">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-676">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="24041-677">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-677">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="24041-678">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-678">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="24041-679">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-679">AMS</span></span>
* <span data-ttu-id="24041-680">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-680">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="24041-681">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-681">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-682">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-682">Appservice</span></span>
* <span data-ttu-id="24041-683">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-683">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="24041-684">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-684">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="24041-685">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-685">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="24041-686">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-686">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="24041-687">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-687">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-688">Botservice</span><span class="sxs-lookup"><span data-stu-id="24041-688">Botservice</span></span>
* <span data-ttu-id="24041-689">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-689">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="24041-690">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-690">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="24041-691">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-691">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="24041-692">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-692">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="24041-693">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-693">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="24041-694">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-694">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="24041-695">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-695">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="24041-696">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-696">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="24041-697">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="24041-697">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="24041-698">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-698">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="24041-699">Key Vault</span><span class="sxs-lookup"><span data-stu-id="24041-699">Key Vault</span></span>
* <span data-ttu-id="24041-700">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-700">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-701">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-701">Monitor</span></span>
* <span data-ttu-id="24041-702">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-702">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="24041-703">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-703">Network</span></span>
* <span data-ttu-id="24041-704">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-704">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="24041-705">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-705">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="24041-706">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-706">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="24041-707">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-707">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="24041-708">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="24041-708">Policy Insights</span></span>
* <span data-ttu-id="24041-709">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-709">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-710">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-710">RDBMS</span></span>
* <span data-ttu-id="24041-711">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-711">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="24041-712">Redis</span><span class="sxs-lookup"><span data-stu-id="24041-712">Redis</span></span>
* <span data-ttu-id="24041-713">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-713">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="24041-714">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-714">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="24041-715">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-715">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="24041-716">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-716">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="24041-717">[호환성이 손상되는 변경] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-717">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="24041-718">[호환성이 손상되는 변경] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-718">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="24041-719">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="24041-719">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="24041-720">역할</span><span class="sxs-lookup"><span data-stu-id="24041-720">Role</span></span>
* <span data-ttu-id="24041-721">[호환성이 손상되는 변경] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-721">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="24041-722">SQL VM</span><span class="sxs-lookup"><span data-stu-id="24041-722">SQL VM</span></span>
* <span data-ttu-id="24041-723">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-723">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="24041-724">VM</span><span class="sxs-lookup"><span data-stu-id="24041-724">VM</span></span>
* <span data-ttu-id="24041-725">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-725">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="24041-726">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-726">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="24041-727">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-727">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="24041-728">[호환성이 손상되는 변경] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-728">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="24041-729">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="24041-729">January 31, 2019</span></span>

<span data-ttu-id="24041-730">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="24041-730">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="24041-731">코어</span><span class="sxs-lookup"><span data-stu-id="24041-731">Core</span></span>

* <span data-ttu-id="24041-732">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="24041-732">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="24041-733">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="24041-733">January 28, 2019</span></span>

<span data-ttu-id="24041-734">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="24041-734">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="24041-735">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-735">ACR</span></span>
* <span data-ttu-id="24041-736">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-736">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="24041-737">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-737">ACS</span></span>
* <span data-ttu-id="24041-738">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="24041-738">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="24041-739">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-739">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="24041-740">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-740">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="24041-741">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-741">AMS</span></span>
* <span data-ttu-id="24041-742">[호환성이 손상되는 변경] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-742">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="24041-743">[호환성이 손상되는 변경] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-743">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-744">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-744">Appservice</span></span>
* <span data-ttu-id="24041-745">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-745">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="24041-746">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-746">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="24041-747">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-747">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="24041-748">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-748">Container</span></span>
* <span data-ttu-id="24041-749">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-749">Added `container start` command</span></span>
* <span data-ttu-id="24041-750">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-750">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="24041-751">EventGrid</span><span class="sxs-lookup"><span data-stu-id="24041-751">EventGrid</span></span>
* <span data-ttu-id="24041-752">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-752">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="24041-753">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-753">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="24041-754">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-754">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="24041-755">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-755">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="24041-756">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-756">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-757">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-757">HDInsight</span></span>
* <span data-ttu-id="24041-758">[호환성이 손상되는 변경] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-758">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="24041-759">[호환성이 손상되는 변경] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-759">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="24041-760">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-760">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="24041-761">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-761">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="24041-762">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-762">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="24041-763">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-763">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="24041-764">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-764">IoT</span></span>
* <span data-ttu-id="24041-765">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-765">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="24041-766">Kusto</span><span class="sxs-lookup"><span data-stu-id="24041-766">Kusto</span></span>
* <span data-ttu-id="24041-767">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-767">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-768">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-768">Monitor</span></span>
* <span data-ttu-id="24041-769">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-769">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="24041-770">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-770">Profile</span></span>
* <span data-ttu-id="24041-771">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-771">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="24041-772">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-772">Network</span></span>
* <span data-ttu-id="24041-773">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-773">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="24041-774">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-774">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="24041-775">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-775">Resource</span></span>
* <span data-ttu-id="24041-776">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-776">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="24041-777">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-777">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="24041-778">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="24041-778">SQL Virtual Machine</span></span>
* <span data-ttu-id="24041-779">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-779">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="24041-780">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-780">Storage</span></span>
* <span data-ttu-id="24041-781">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-781">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="24041-782">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-782">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="24041-783">VM</span><span class="sxs-lookup"><span data-stu-id="24041-783">VM</span></span>
* <span data-ttu-id="24041-784">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-784">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="24041-785">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-785">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="24041-786">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="24041-786">January 15, 2019</span></span>

<span data-ttu-id="24041-787">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="24041-787">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="24041-788">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-788">ACR</span></span>
* <span data-ttu-id="24041-789">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-789">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="24041-790">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-790">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="24041-791">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="24041-791">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="24041-792">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-792">ACS</span></span>
* <span data-ttu-id="24041-793">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-793">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-794">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-794">Appservice</span></span>
* <span data-ttu-id="24041-795">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-795">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="24041-796">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-796">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="24041-797">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-797">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="24041-798">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-798">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-799">Botservice</span><span class="sxs-lookup"><span data-stu-id="24041-799">Botservice</span></span>
* <span data-ttu-id="24041-800">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-800">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="24041-801">구성</span><span class="sxs-lookup"><span data-stu-id="24041-801">Configure</span></span>
* <span data-ttu-id="24041-802">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-802">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-803">CosmosDB</span></span>
* <span data-ttu-id="24041-804">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-804">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-805">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-805">HDInsight</span></span>
* <span data-ttu-id="24041-806">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-806">Added commands for managing applications</span></span>
* <span data-ttu-id="24041-807">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-807">Added commands for managing script actions</span></span>
* <span data-ttu-id="24041-808">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-808">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="24041-809">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-809">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="24041-810">[호환성이 손상되는 변경] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-810">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="24041-811">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-811">Network</span></span>
* <span data-ttu-id="24041-812">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-812">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="24041-813">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-813">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="24041-814">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-814">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="24041-815">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-815">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="24041-816">역할</span><span class="sxs-lookup"><span data-stu-id="24041-816">Role</span></span>
* <span data-ttu-id="24041-817">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-817">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="24041-818">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-818">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="24041-819">보안</span><span class="sxs-lookup"><span data-stu-id="24041-819">Security</span></span>
* <span data-ttu-id="24041-820">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-820">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="24041-821">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-821">Storage</span></span>
* <span data-ttu-id="24041-822">[호환성이 손상되는 변경] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-822">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="24041-823">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-823">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="24041-824">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-824">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="24041-825">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-825">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="24041-826">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-826">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="24041-827">VM</span><span class="sxs-lookup"><span data-stu-id="24041-827">VM</span></span>
* <span data-ttu-id="24041-828">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-828">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="24041-829">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-829">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="24041-830">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-830">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="24041-831">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-831">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="24041-832">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-832">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="24041-833">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-833">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="24041-834">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="24041-834">December 20, 2018</span></span>

<span data-ttu-id="24041-835">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="24041-835">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="24041-836">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-836">Appservice</span></span>
* <span data-ttu-id="24041-837">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-837">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="24041-838">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-838">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="24041-839">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-839">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="24041-840">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="24041-840">IoTCentral</span></span>
* <span data-ttu-id="24041-841">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-841">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="24041-842">역할</span><span class="sxs-lookup"><span data-stu-id="24041-842">Role</span></span>
* <span data-ttu-id="24041-843">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-843">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="24041-844">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-844">SQL</span></span>
* <span data-ttu-id="24041-845">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-845">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="24041-846">VM</span><span class="sxs-lookup"><span data-stu-id="24041-846">VM</span></span>
* <span data-ttu-id="24041-847">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-847">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="24041-848">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="24041-848">December 18, 2018</span></span>

<span data-ttu-id="24041-849">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="24041-849">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="24041-850">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-850">ACR</span></span>
* <span data-ttu-id="24041-851">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-851">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="24041-852">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="24041-852">Condensed the table layout for task list</span></span>
* <span data-ttu-id="24041-853">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-853">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="24041-854">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-854">ACS</span></span>
* <span data-ttu-id="24041-855">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="24041-855">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="24041-856">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="24041-856">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="24041-857">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-857">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="24041-858">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-858">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="24041-859">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-859">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="24041-860">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="24041-860">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-861">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-861">Appservice</span></span>
* <span data-ttu-id="24041-862">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="24041-862">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="24041-863">Botservice</span><span class="sxs-lookup"><span data-stu-id="24041-863">Botservice</span></span>
* <span data-ttu-id="24041-864">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-864">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="24041-865">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="24041-865">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="24041-866">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="24041-866">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="24041-867">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="24041-867">Reduced Kudu network calls</span></span>
* <span data-ttu-id="24041-868">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="24041-868">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-869">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-869">Consumption</span></span>
* <span data-ttu-id="24041-870">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-870">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-871">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-871">CosmosDB</span></span>
* <span data-ttu-id="24041-872">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-872">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="24041-873">지도</span><span class="sxs-lookup"><span data-stu-id="24041-873">Maps</span></span>
* <span data-ttu-id="24041-874">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-874">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="24041-875">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-875">Network</span></span>
* <span data-ttu-id="24041-876">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-876">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="24041-877">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="24041-877">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="24041-878">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-878">Resource</span></span>
* <span data-ttu-id="24041-879">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-879">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="24041-880">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-880">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-881">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-881">Storage</span></span>
*  <span data-ttu-id="24041-882">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-882">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-883">VM</span><span class="sxs-lookup"><span data-stu-id="24041-883">VM</span></span>
* <span data-ttu-id="24041-884">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-884">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="24041-885">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="24041-885">December 4, 2018</span></span>

<span data-ttu-id="24041-886">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="24041-886">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="24041-887">코어</span><span class="sxs-lookup"><span data-stu-id="24041-887">Core</span></span>
* <span data-ttu-id="24041-888">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-888">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="24041-889">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-889">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-890">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-890">Appservice</span></span>
* <span data-ttu-id="24041-891">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-891">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="24041-892">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-892">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="24041-893">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-893">Network</span></span>
* <span data-ttu-id="24041-894">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-894">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="24041-895">역할</span><span class="sxs-lookup"><span data-stu-id="24041-895">Role</span></span>
* <span data-ttu-id="24041-896">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-896">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="24041-897">VM</span><span class="sxs-lookup"><span data-stu-id="24041-897">VM</span></span>
* <span data-ttu-id="24041-898">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-898">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="24041-899">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-899">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="24041-900">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-900">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="24041-901">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-901">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="24041-902">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="24041-902">November 20, 2018</span></span>

<span data-ttu-id="24041-903">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="24041-903">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="24041-904">코어</span><span class="sxs-lookup"><span data-stu-id="24041-904">Core</span></span>
* <span data-ttu-id="24041-905">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="24041-905">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="24041-906">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-906">ACR</span></span>
* <span data-ttu-id="24041-907">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="24041-907">Added context token to task step</span></span>
* <span data-ttu-id="24041-908">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-908">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="24041-909">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="24041-909">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-910">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-910">Appservice</span></span>
* <span data-ttu-id="24041-911">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-911">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="24041-912">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-912">Updated the default `node_version`.</span></span> <span data-ttu-id="24041-913">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-913">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="24041-914">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="24041-914">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="24041-915">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-915">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="24041-916">IotCentral</span><span class="sxs-lookup"><span data-stu-id="24041-916">IotCentral</span></span>
* <span data-ttu-id="24041-917">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="24041-917">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-918">KeyVault</span><span class="sxs-lookup"><span data-stu-id="24041-918">KeyVault</span></span>
* <span data-ttu-id="24041-919">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-919">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="24041-920">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-920">Network</span></span>
* <span data-ttu-id="24041-921">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-921">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="24041-922">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="24041-922">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="24041-923">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-923">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="24041-924">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="24041-924">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-925">Rdbms</span><span class="sxs-lookup"><span data-stu-id="24041-925">Rdbms</span></span>
* <span data-ttu-id="24041-926">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-926">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="24041-927">Rbac</span><span class="sxs-lookup"><span data-stu-id="24041-927">Rbac</span></span>
* <span data-ttu-id="24041-928">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-928">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="24041-929">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-929">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="24041-930">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-930">Storage</span></span>
* <span data-ttu-id="24041-931">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-931">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="24041-932">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-932">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="24041-933">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-933">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="24041-934">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-934">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="24041-935">VM</span><span class="sxs-lookup"><span data-stu-id="24041-935">VM</span></span>
* <span data-ttu-id="24041-936">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-936">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="24041-937">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-937">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="24041-938">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="24041-938">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="24041-939">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-939">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="24041-940">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-940">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="24041-941">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-941">Added `snapshot wait` command</span></span>
* <span data-ttu-id="24041-942">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-942">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="24041-943">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="24041-943">November 6, 2018</span></span>

<span data-ttu-id="24041-944">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="24041-944">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="24041-945">코어</span><span class="sxs-lookup"><span data-stu-id="24041-945">Core</span></span>
* <span data-ttu-id="24041-946">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-946">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="24041-947">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-947">ACR</span></span>
* <span data-ttu-id="24041-948">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-948">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="24041-949">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-949">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="24041-950">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-950">ACS</span></span>
* <span data-ttu-id="24041-951">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-951">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="24041-952">Advisor</span><span class="sxs-lookup"><span data-stu-id="24041-952">Advisor</span></span>
* <span data-ttu-id="24041-953">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-953">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="24041-954">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-954">AMS</span></span>
* <span data-ttu-id="24041-955">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="24041-955">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="24041-956">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="24041-956">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="24041-957">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-957">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="24041-958">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-958">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="24041-959">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-959">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="24041-960">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-960">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="24041-961">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-961">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="24041-962">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="24041-962">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="24041-963">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-963">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="24041-964">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-964">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="24041-965">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="24041-965">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="24041-966">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="24041-966">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="24041-967">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="24041-967">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="24041-968">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="24041-968">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="24041-969">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-969">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="24041-970">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-970">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="24041-971">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-971">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-972">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-972">AppService</span></span>
* <span data-ttu-id="24041-973">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-973">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="24041-974">구성</span><span class="sxs-lookup"><span data-stu-id="24041-974">Configure</span></span>
* <span data-ttu-id="24041-975">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-975">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="24041-976">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-976">Container</span></span>
* <span data-ttu-id="24041-977">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-977">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="24041-978">EventHub</span><span class="sxs-lookup"><span data-stu-id="24041-978">EventHub</span></span>
* <span data-ttu-id="24041-979">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-979">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-980">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-980">Interactive</span></span>
* <span data-ttu-id="24041-981">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="24041-981">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-982">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-982">Monitor</span></span>
* <span data-ttu-id="24041-983">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-983">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="24041-984">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-984">Network</span></span>
* <span data-ttu-id="24041-985">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-985">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="24041-986">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-986">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="24041-987">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-987">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="24041-988">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-988">Profile</span></span>
* <span data-ttu-id="24041-989">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-989">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-990">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-990">RDBMS</span></span>
* <span data-ttu-id="24041-991">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-991">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="24041-992">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-992">Resource</span></span>
* <span data-ttu-id="24041-993">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-993">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="24041-994">역할</span><span class="sxs-lookup"><span data-stu-id="24041-994">Role</span></span>
* <span data-ttu-id="24041-995">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-995">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="24041-996">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-996">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="24041-997">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-997">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="24041-998">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-998">Storage</span></span>
* <span data-ttu-id="24041-999">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-999">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1000">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1000">VM</span></span>
* <span data-ttu-id="24041-1001">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1001">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="24041-1002">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1002">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="24041-1003">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1003">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="24041-1004">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1004">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="24041-1005">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="24041-1005">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="24041-1006">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1006">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="24041-1007">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="24041-1007">October 23, 2018</span></span>

<span data-ttu-id="24041-1008">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="24041-1008">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="24041-1009">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1009">Core</span></span>
* <span data-ttu-id="24041-1010">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1010">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="24041-1011">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1011">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1012">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1012">ACR</span></span>
* <span data-ttu-id="24041-1013">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1013">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-1014">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-1014">CDN</span></span>
* <span data-ttu-id="24041-1015">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1015">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="24041-1016">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1016">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="24041-1017">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1017">Container</span></span>
* <span data-ttu-id="24041-1018">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1018">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="24041-1019">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1019">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="24041-1020">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1020">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="24041-1021">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1021">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="24041-1022">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1022">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="24041-1023">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1023">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="24041-1024">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1024">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-1025">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-1025">CosmosDB</span></span>
* <span data-ttu-id="24041-1026">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1026">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1027">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1027">Interactive</span></span>
* <span data-ttu-id="24041-1028">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1028">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="24041-1029">IoT Central</span><span class="sxs-lookup"><span data-stu-id="24041-1029">IoT Central</span></span>
* <span data-ttu-id="24041-1030">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1030">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="24041-1031">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1031">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-1032">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-1032">Monitor</span></span>
* <span data-ttu-id="24041-1033">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="24041-1033">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="24041-1034">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1034">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="24041-1035">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1035">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="24041-1036">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1036">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="24041-1037">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1037">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="24041-1038">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1038">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="24041-1039">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="24041-1039">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="24041-1040">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1040">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="24041-1041">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1041">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="24041-1042">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1042">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="24041-1043">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1043">Network</span></span>
* <span data-ttu-id="24041-1044">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1044">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="24041-1045">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1045">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="24041-1046">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24041-1046">ServiceBus</span></span>
* <span data-ttu-id="24041-1047">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1047">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1048">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1048">SQL</span></span>
* <span data-ttu-id="24041-1049">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1049">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1050">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1050">Storage</span></span>
* <span data-ttu-id="24041-1051">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1051">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="24041-1052">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1052">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1053">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1053">VM</span></span>
* <span data-ttu-id="24041-1054">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1054">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="24041-1055">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1055">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="24041-1056">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1056">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="24041-1057">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="24041-1057">October 16, 2018</span></span>

<span data-ttu-id="24041-1058">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="24041-1058">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1059">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1059">VM</span></span>
* <span data-ttu-id="24041-1060">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1060">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="24041-1061">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="24041-1061">October 9, 2018</span></span>

<span data-ttu-id="24041-1062">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="24041-1062">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="24041-1063">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1063">Core</span></span>
* <span data-ttu-id="24041-1064">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="24041-1064">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1065">ACR</span></span>
* <span data-ttu-id="24041-1066">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1066">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1067">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1067">ACS</span></span>
* <span data-ttu-id="24041-1068">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="24041-1068">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="24041-1069">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1069">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="24041-1070">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1070">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="24041-1071">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="24041-1071">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="24041-1072">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1072">Container</span></span>
* <span data-ttu-id="24041-1073">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1073">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="24041-1074">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1074">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="24041-1075">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="24041-1075">Event Hub</span></span>
* <span data-ttu-id="24041-1076">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1076">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="24041-1077">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1077">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="24041-1078">확장</span><span class="sxs-lookup"><span data-stu-id="24041-1078">Extensions</span></span>
* <span data-ttu-id="24041-1079">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1079">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="24041-1080">HDInsight</span><span class="sxs-lookup"><span data-stu-id="24041-1080">HDInsight</span></span>
* <span data-ttu-id="24041-1081">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1081">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="24041-1082">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-1082">IoT</span></span>
* <span data-ttu-id="24041-1083">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1083">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-1084">KeyVault</span><span class="sxs-lookup"><span data-stu-id="24041-1084">KeyVault</span></span>
* <span data-ttu-id="24041-1085">최신 API 프로필에 keyvault 스토리지 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1085">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="24041-1086">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1086">Network</span></span>
* <span data-ttu-id="24041-1087">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1087">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="24041-1088">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="24041-1088">See #6052</span></span>
* <span data-ttu-id="24041-1089">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="24041-1089">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="24041-1090">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1090">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="24041-1091">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1091">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="24041-1092">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1092">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="24041-1093">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1093">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="24041-1094">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1094">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="24041-1095">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1095">Role</span></span>
* <span data-ttu-id="24041-1096">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1096">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="24041-1097">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1097">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="24041-1098">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1098">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="24041-1099">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1099">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="24041-1100">Service Bus</span><span class="sxs-lookup"><span data-stu-id="24041-1100">Service Bus</span></span>
* <span data-ttu-id="24041-1101">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1101">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1102">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1102">VM</span></span>
* <span data-ttu-id="24041-1103">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1103">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="24041-1104">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1104">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="24041-1105">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1105">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="24041-1106">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1106">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="24041-1107">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1107">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="24041-1108">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1108">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="24041-1109">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="24041-1109">September 21, 2018</span></span>

<span data-ttu-id="24041-1110">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="24041-1110">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1111">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1111">ACR</span></span>
* <span data-ttu-id="24041-1112">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1112">Added ACR Task commands</span></span>
* <span data-ttu-id="24041-1113">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1113">Added quick run command</span></span>
* <span data-ttu-id="24041-1114">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1114">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="24041-1115">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1115">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="24041-1116">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1116">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="24041-1117">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1117">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1118">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1118">ACS</span></span>
* <span data-ttu-id="24041-1119">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1119">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="24041-1120">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1120">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1121">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1121">AppService</span></span>

* <span data-ttu-id="24041-1122">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1122">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="24041-1123">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1123">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="24041-1124">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1124">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="24041-1125">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1125">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1126">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1126">Batch</span></span>
* <span data-ttu-id="24041-1127">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1127">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="24041-1128">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1128">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="24041-1129">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1129">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="24041-1130">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1130">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="24041-1131">Batch AI</span><span class="sxs-lookup"><span data-stu-id="24041-1131">Batch AI</span></span> 
* <span data-ttu-id="24041-1132">`batchai cluster create` 명령에서 자동 스토리지 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1132">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="24041-1133">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="24041-1133">Cognitive Services</span></span>
* <span data-ttu-id="24041-1134">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1134">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="24041-1135">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1135">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="24041-1136">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1136">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="24041-1137">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1137">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="24041-1138">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1138">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="24041-1139">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1139">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="24041-1140">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1140">Container</span></span>
* <span data-ttu-id="24041-1141">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1141">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="24041-1142">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1142">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="24041-1143">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1143">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="24041-1144">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1144">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="24041-1145">Datalake</span><span class="sxs-lookup"><span data-stu-id="24041-1145">Datalake</span></span>
* <span data-ttu-id="24041-1146">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1146">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="24041-1147">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="24041-1147">Interactive Shell</span></span>
* <span data-ttu-id="24041-1148">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1148">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="24041-1149">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1149">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="24041-1150">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-1150">IoT</span></span>
* <span data-ttu-id="24041-1151">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1151">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="24041-1152">Key Vault</span><span class="sxs-lookup"><span data-stu-id="24041-1152">Key Vault</span></span>
* <span data-ttu-id="24041-1153">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1153">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="24041-1154">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1154">Network</span></span>
* <span data-ttu-id="24041-1155">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1155">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="24041-1156">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1156">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="24041-1157">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1157">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="24041-1158">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1158">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="24041-1159">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1159">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="24041-1160">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1160">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="24041-1161">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1161">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="24041-1162">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1162">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="24041-1163">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1163">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="24041-1164">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1164">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="24041-1165">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1165">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="24041-1166">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1166">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="24041-1167">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1167">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="24041-1168">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="24041-1168">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="24041-1169">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1169">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="24041-1170">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1170">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="24041-1171">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1171">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="24041-1172">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1172">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-1173">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-1173">RDBMS</span></span>
* <span data-ttu-id="24041-1174">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1174">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="24041-1175">예약</span><span class="sxs-lookup"><span data-stu-id="24041-1175">Reservation</span></span>
* <span data-ttu-id="24041-1176">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1176">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="24041-1177">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1177">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="24041-1178">앱 관리</span><span class="sxs-lookup"><span data-stu-id="24041-1178">Manage App</span></span>
* <span data-ttu-id="24041-1179">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1179">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="24041-1180">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1180">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="24041-1181">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1181">Role</span></span>
* <span data-ttu-id="24041-1182">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1182">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="24041-1183">SignalR</span><span class="sxs-lookup"><span data-stu-id="24041-1183">SignalR</span></span>
* <span data-ttu-id="24041-1184">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1184">First release</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1185">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1185">Storage</span></span>
* <span data-ttu-id="24041-1186">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1186">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="24041-1187">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1187">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1188">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1188">VM</span></span>
* <span data-ttu-id="24041-1189">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="24041-1189">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="24041-1190">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1190">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="24041-1191">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="24041-1191">August 28, 2018</span></span>

<span data-ttu-id="24041-1192">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="24041-1192">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="24041-1193">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1193">Core</span></span>

* <span data-ttu-id="24041-1194">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1194">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="24041-1195">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1195">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1196">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1196">ACR</span></span>

* <span data-ttu-id="24041-1197">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1197">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="24041-1198">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1198">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1199">ACS</span></span>

* <span data-ttu-id="24041-1200">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1200">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="24041-1201">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1201">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1202">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1202">AppService</span></span>

* <span data-ttu-id="24041-1203">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1203">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="24041-1204">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1204">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="24041-1205">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1205">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="24041-1206">Backup</span><span class="sxs-lookup"><span data-stu-id="24041-1206">Backup</span></span>

* <span data-ttu-id="24041-1207">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1207">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="24041-1208">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="24041-1208">Bot Service</span></span>

* <span data-ttu-id="24041-1209">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1209">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="24041-1210">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="24041-1210">Cognitive Services</span></span>

* <span data-ttu-id="24041-1211">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1211">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="24041-1212">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-1212">IoT</span></span>

* <span data-ttu-id="24041-1213">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1213">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-1214">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-1214">Monitor</span></span>

* <span data-ttu-id="24041-1215">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1215">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="24041-1216">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="24041-1216">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="24041-1217">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1217">Network</span></span>

* <span data-ttu-id="24041-1218">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1218">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1219">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1219">Resource</span></span>

* <span data-ttu-id="24041-1220">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1220">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1221">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1221">Storage</span></span>

* <span data-ttu-id="24041-1222">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1222">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1223">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1223">VM</span></span>

* <span data-ttu-id="24041-1224">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1224">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="24041-1225">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="24041-1225">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="24041-1226">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="24041-1226">Auguest 14, 2018</span></span>

<span data-ttu-id="24041-1227">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="24041-1227">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="24041-1228">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1228">Core</span></span>

* <span data-ttu-id="24041-1229">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1229">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="24041-1230">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="24041-1230">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="24041-1231">원격 분석</span><span class="sxs-lookup"><span data-stu-id="24041-1231">Telemetry</span></span>

* <span data-ttu-id="24041-1232">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="24041-1232">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1233">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1233">ACR</span></span>

* <span data-ttu-id="24041-1234">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1234">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="24041-1235">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1235">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1236">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1236">ACS</span></span>

* <span data-ttu-id="24041-1237">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1237">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="24041-1238">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1238">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="24041-1239">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1239">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="24041-1240">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1240">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="24041-1241">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1241">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="24041-1242">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1242">AppService</span></span>

* <span data-ttu-id="24041-1243">외부 리소스 그룹에 스토리지 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1243">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="24041-1244">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1244">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-1245">BatchAI</span><span class="sxs-lookup"><span data-stu-id="24041-1245">BatchAI</span></span>

* <span data-ttu-id="24041-1246">자동 스토리지 계정 만들기가 &quot;리소스 *그룹*&quot;을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1246">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="24041-1247">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1247">Container</span></span>

* <span data-ttu-id="24041-1248">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1248">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="24041-1249">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-1249">IoT</span></span>

* <span data-ttu-id="24041-1250">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="24041-1250">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="24041-1251">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1251">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="24041-1252">Iot Central</span><span class="sxs-lookup"><span data-stu-id="24041-1252">Iot Central</span></span>

* <span data-ttu-id="24041-1253">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1253">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-1254">KeyVault</span><span class="sxs-lookup"><span data-stu-id="24041-1254">KeyVault</span></span>


* <span data-ttu-id="24041-1255">스토리지 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1255">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="24041-1256">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1256">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="24041-1257">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1257">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="24041-1258">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1258">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="24041-1259">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1259">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="24041-1260">릴레이</span><span class="sxs-lookup"><span data-stu-id="24041-1260">Relay</span></span>

* <span data-ttu-id="24041-1261">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1261">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1262">Sql</span><span class="sxs-lookup"><span data-stu-id="24041-1262">Sql</span></span>

* <span data-ttu-id="24041-1263">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1263">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1264">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1264">Storage</span></span>

* <span data-ttu-id="24041-1265">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="24041-1265">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="24041-1266">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1266">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="24041-1267">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1267">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="24041-1268">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="24041-1268">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="24041-1269">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1269">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1270">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1270">VM</span></span>

* <span data-ttu-id="24041-1271">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1271">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="24041-1272">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="24041-1272">July 31, 2018</span></span>

<span data-ttu-id="24041-1273">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="24041-1273">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1274">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1274">ACR</span></span>

* <span data-ttu-id="24041-1275">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1275">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="24041-1276">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1276">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1277">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1277">ACS</span></span>

* <span data-ttu-id="24041-1278">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1278">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1279">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1279">Batch</span></span>

* <span data-ttu-id="24041-1280">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1280">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="24041-1281">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1281">Container</span></span>

* <span data-ttu-id="24041-1282">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1282">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="24041-1283">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1283">Network</span></span>

* <span data-ttu-id="24041-1284">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1284">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="24041-1285">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1285">Resource</span></span>

* <span data-ttu-id="24041-1286">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="24041-1286">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="24041-1287">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1287">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="24041-1288">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1288">Role</span></span>

* <span data-ttu-id="24041-1289">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1289">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="24041-1290">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1290">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="24041-1291">검색</span><span class="sxs-lookup"><span data-stu-id="24041-1291">Search</span></span>

* <span data-ttu-id="24041-1292">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1292">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="24041-1293">Service Bus</span><span class="sxs-lookup"><span data-stu-id="24041-1293">Service Bus</span></span>

* <span data-ttu-id="24041-1294">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1294">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="24041-1295">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1295">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="24041-1296">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="24041-1296">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="24041-1297">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="24041-1297">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1298">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1298">Storage</span></span>

* <span data-ttu-id="24041-1299">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1299">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="24041-1300">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="24041-1300">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1301">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1301">VM</span></span>

* <span data-ttu-id="24041-1302">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1302">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="24041-1303">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1303">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="24041-1304">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1304">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="24041-1305">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1305">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="24041-1306">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="24041-1306">July 18, 2018</span></span>

<span data-ttu-id="24041-1307">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="24041-1307">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="24041-1308">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1308">Core</span></span>

* <span data-ttu-id="24041-1309">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1309">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="24041-1310">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1310">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="24041-1311">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1311">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1312">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1312">ACR</span></span>

* <span data-ttu-id="24041-1313">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1313">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="24041-1314">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1314">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="24041-1315">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1315">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="24041-1316">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1316">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1317">ACS</span></span>

* <span data-ttu-id="24041-1318">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1318">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1319">AppService</span></span>

* <span data-ttu-id="24041-1320">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1320">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1321">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1321">Batch</span></span>

* <span data-ttu-id="24041-1322">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1322">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="24041-1323">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1323">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="24041-1324">Batch AI</span><span class="sxs-lookup"><span data-stu-id="24041-1324">Batch AI</span></span>

* <span data-ttu-id="24041-1325">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1325">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="24041-1326">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1326">Container</span></span>

* <span data-ttu-id="24041-1327">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1327">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="24041-1328">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1328">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="24041-1329">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1329">Network</span></span>

* <span data-ttu-id="24041-1330">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1330">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="24041-1331">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1331">Added `network nic wait`</span></span>
* <span data-ttu-id="24041-1332">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1332">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="24041-1333">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1333">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="24041-1334">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1334">Resource</span></span>

* <span data-ttu-id="24041-1335">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1335">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="24041-1336">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1336">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="24041-1337">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1337">Added `deployment wait` command</span></span>
* <span data-ttu-id="24041-1338">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1338">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1339">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1339">SQL</span></span>

* <span data-ttu-id="24041-1340">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1340">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="24041-1341">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1341">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="24041-1342">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="24041-1342">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1343">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1343">Storage</span></span>

* <span data-ttu-id="24041-1344">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1344">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1345">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1345">VM</span></span>

* <span data-ttu-id="24041-1346">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1346">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="24041-1347">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1347">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="24041-1348">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1348">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="24041-1349">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="24041-1349">July 3, 2018</span></span>

<span data-ttu-id="24041-1350">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="24041-1350">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="24041-1351">AKS</span><span class="sxs-lookup"><span data-stu-id="24041-1351">AKS</span></span>

* <span data-ttu-id="24041-1352">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1352">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="24041-1353">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="24041-1353">July 3, 2018</span></span>

<span data-ttu-id="24041-1354">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="24041-1354">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="24041-1355">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1355">Core</span></span>

* <span data-ttu-id="24041-1356">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1356">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1357">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1357">ACR</span></span>

* <span data-ttu-id="24041-1358">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1358">Added polling build status</span></span>
* <span data-ttu-id="24041-1359">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1359">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="24041-1360">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1360">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1361">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1361">ACS</span></span>

* <span data-ttu-id="24041-1362">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1362">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="24041-1363">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1363">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="24041-1364">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="24041-1364">Updated options for `aks browse` command.</span></span> <span data-ttu-id="24041-1365">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1365">Added `--listen-port` support</span></span>
* <span data-ttu-id="24041-1366">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1366">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="24041-1367">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="24041-1367">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="24041-1368">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1368">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1369">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1369">AppService</span></span>

* <span data-ttu-id="24041-1370">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1370">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="24041-1371">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1371">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="24041-1372">Backup</span><span class="sxs-lookup"><span data-stu-id="24041-1372">Backup</span></span>

* <span data-ttu-id="24041-1373">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1373">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-1374">BatchAI</span><span class="sxs-lookup"><span data-stu-id="24041-1374">BatchAI</span></span>

* <span data-ttu-id="24041-1375">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1375">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="24041-1376">클라우드</span><span class="sxs-lookup"><span data-stu-id="24041-1376">Cloud</span></span>

* <span data-ttu-id="24041-1377">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1377">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="24041-1378">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1378">Container</span></span>

* <span data-ttu-id="24041-1379">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1379">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="24041-1380">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1380">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="24041-1381">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1381">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1382">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1382">Extension</span></span>

* <span data-ttu-id="24041-1383">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1383">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="24041-1384">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1384">Network</span></span>

* <span data-ttu-id="24041-1385">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="24041-1385">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-1386">Rdbms</span><span class="sxs-lookup"><span data-stu-id="24041-1386">Rdbms</span></span>

* <span data-ttu-id="24041-1387">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1387">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1388">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1388">Resource</span></span>

* <span data-ttu-id="24041-1389">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1389">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1390">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1390">VM</span></span>

* <span data-ttu-id="24041-1391">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1391">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="24041-1392">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="24041-1392">June 25, 2018</span></span>

<span data-ttu-id="24041-1393">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="24041-1393">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="24041-1394">CLI</span><span class="sxs-lookup"><span data-stu-id="24041-1394">CLI</span></span>

* <span data-ttu-id="24041-1395">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1395">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="24041-1396">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="24041-1396">June 19, 2018</span></span>

<span data-ttu-id="24041-1397">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="24041-1397">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="24041-1398">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1398">Core</span></span>

* <span data-ttu-id="24041-1399">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1399">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1400">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1400">ACR</span></span>

* <span data-ttu-id="24041-1401">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1401">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="24041-1402">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1402">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1403">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1403">ACS</span></span>

* <span data-ttu-id="24041-1404">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="24041-1404">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="24041-1405">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1405">Added `--update` support</span></span>
* <span data-ttu-id="24041-1406">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1406">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="24041-1407">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="24041-1407">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="24041-1408">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1408">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="24041-1409">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1409">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="24041-1410">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1410">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="24041-1411">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1411">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1412">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1412">AppService</span></span>

* <span data-ttu-id="24041-1413">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1413">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="24041-1414">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1414">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1415">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1415">Batch</span></span>

* <span data-ttu-id="24041-1416">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1416">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="24041-1417">Batch AI</span><span class="sxs-lookup"><span data-stu-id="24041-1417">Batch AI</span></span>

* <span data-ttu-id="24041-1418">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="24041-1418">Added support for workspaces.</span></span> <span data-ttu-id="24041-1419">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1419">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="24041-1420">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="24041-1420">Added support for experiments.</span></span> <span data-ttu-id="24041-1421">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1421">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="24041-1422">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1422">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="24041-1423">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="24041-1423">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="24041-1424">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1424">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="24041-1425">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1425">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="24041-1426">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="24041-1426">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="24041-1427">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="24041-1427">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="24041-1428">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="24041-1428">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="24041-1429">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="24041-1429">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="24041-1430">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="24041-1430">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="24041-1431">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="24041-1431">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="24041-1432">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="24041-1432">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="24041-1433">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1433">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="24041-1434">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="24041-1434">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="24041-1435">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="24041-1435">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="24041-1436">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="24041-1436">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="24041-1437">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="24041-1437">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="24041-1438">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="24041-1438">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="24041-1439">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="24041-1439">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="24041-1440">지도</span><span class="sxs-lookup"><span data-stu-id="24041-1440">Maps</span></span>

* <span data-ttu-id="24041-1441">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1441">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="24041-1442">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1442">Network</span></span>

* <span data-ttu-id="24041-1443">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1443">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="24041-1444">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1444">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="24041-1445">#6502</span><span class="sxs-lookup"><span data-stu-id="24041-1445">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="24041-1446">예약</span><span class="sxs-lookup"><span data-stu-id="24041-1446">Reservations</span></span>

* <span data-ttu-id="24041-1447">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1447">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="24041-1448">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1448">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="24041-1449">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="24041-1449">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="24041-1450">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1450">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="24041-1451">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1451">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="24041-1452">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1452">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="24041-1453">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1453">Role</span></span>

* <span data-ttu-id="24041-1454">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="24041-1454">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1455">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1455">SQL</span></span>

* <span data-ttu-id="24041-1456">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1456">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1457">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1457">Storage</span></span>

* <span data-ttu-id="24041-1458">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1458">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1459">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1459">VM</span></span>

* <span data-ttu-id="24041-1460">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="24041-1460">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="24041-1461">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1461">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="24041-1462">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1462">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="24041-1463">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="24041-1463">June 13, 2018</span></span>

<span data-ttu-id="24041-1464">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="24041-1464">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="24041-1465">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1465">Core</span></span>

* <span data-ttu-id="24041-1466">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="24041-1466">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="24041-1467">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="24041-1467">June 13, 2018</span></span>

<span data-ttu-id="24041-1468">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="24041-1468">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="24041-1469">AKS</span><span class="sxs-lookup"><span data-stu-id="24041-1469">AKS</span></span>

* <span data-ttu-id="24041-1470">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1470">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="24041-1471">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="24041-1471">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="24041-1472">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1472">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="24041-1473">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1473">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="24041-1474">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1474">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1475">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1475">AppService</span></span>

* <span data-ttu-id="24041-1476">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1476">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="24041-1477">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="24041-1477">June 5, 2018</span></span>

<span data-ttu-id="24041-1478">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="24041-1478">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1479">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1479">Interactive</span></span>

* <span data-ttu-id="24041-1480">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1480">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="24041-1481">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="24041-1481">June 5, 2018</span></span>

<span data-ttu-id="24041-1482">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="24041-1482">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="24041-1483">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1483">Core</span></span>

* <span data-ttu-id="24041-1484">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1484">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="24041-1485">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1485">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1486">ACR</span></span>

* <span data-ttu-id="24041-1487">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1487">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="24041-1488">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1488">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="24041-1489">AKS</span><span class="sxs-lookup"><span data-stu-id="24041-1489">AKS</span></span>

* <span data-ttu-id="24041-1490">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="24041-1490">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1491">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1491">Batch</span></span>

* <span data-ttu-id="24041-1492">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="24041-1492">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="24041-1493">IOT</span><span class="sxs-lookup"><span data-stu-id="24041-1493">IOT</span></span>

* <span data-ttu-id="24041-1494">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1494">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="24041-1495">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1495">Network</span></span>

* <span data-ttu-id="24041-1496">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="24041-1496">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="24041-1497">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="24041-1497">Policy Insights</span></span>

* <span data-ttu-id="24041-1498">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1498">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="24041-1499">ARM</span><span class="sxs-lookup"><span data-stu-id="24041-1499">ARM</span></span>

* <span data-ttu-id="24041-1500">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1500">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1501">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1501">SQL</span></span>

* <span data-ttu-id="24041-1502">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="24041-1502">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="24041-1503">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1503">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="24041-1504">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1504">Storage</span></span>

* <span data-ttu-id="24041-1505">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="24041-1505">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1506">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1506">VM</span></span>

* <span data-ttu-id="24041-1507">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1507">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="24041-1508">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1508">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="24041-1509">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1509">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="24041-1510">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="24041-1510">May 22, 2018</span></span>

<span data-ttu-id="24041-1511">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="24041-1511">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="24041-1512">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1512">Core</span></span>

* <span data-ttu-id="24041-1513">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1513">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1514">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1514">ACS</span></span>

* <span data-ttu-id="24041-1515">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1515">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="24041-1516">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1516">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1517">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-1517">AppService</span></span>

* <span data-ttu-id="24041-1518">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1518">Improved generic update commands</span></span>
* <span data-ttu-id="24041-1519">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1519">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="24041-1520">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1520">Container</span></span>

* <span data-ttu-id="24041-1521">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1521">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="24041-1522">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1522">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1523">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1523">Extension</span></span>

* <span data-ttu-id="24041-1524">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1524">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1525">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1525">Interactive</span></span>

* <span data-ttu-id="24041-1526">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-1526">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="24041-1527">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1527">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-1528">KeyVault</span><span class="sxs-lookup"><span data-stu-id="24041-1528">KeyVault</span></span>

* <span data-ttu-id="24041-1529">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="24041-1529">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="24041-1530">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1530">Network</span></span>

* <span data-ttu-id="24041-1531">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1531">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="24041-1532">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1532">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1533">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1533">SQL</span></span>

* <span data-ttu-id="24041-1534">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="24041-1534">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="24041-1535">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="24041-1535">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="24041-1536">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1536">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="24041-1537">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1537">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="24041-1538">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1538">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="24041-1539">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="24041-1539">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="24041-1540">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1540">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="24041-1541">`edition`.</span><span class="sxs-lookup"><span data-stu-id="24041-1541">`edition`.</span></span> <span data-ttu-id="24041-1542">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1542">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="24041-1543">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="24041-1543">`elasticPoolName`.</span></span> <span data-ttu-id="24041-1544">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1544">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="24041-1545">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1545">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="24041-1546">`edition`.</span><span class="sxs-lookup"><span data-stu-id="24041-1546">`edition`.</span></span> <span data-ttu-id="24041-1547">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="24041-1547">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="24041-1548">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="24041-1548">`dtu`.</span></span> <span data-ttu-id="24041-1549">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="24041-1549">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="24041-1550">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="24041-1550">`databaseDtuMin`.</span></span> <span data-ttu-id="24041-1551">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="24041-1551">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="24041-1552">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="24041-1552">`databaseDtuMax`.</span></span> <span data-ttu-id="24041-1553">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="24041-1553">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="24041-1554">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1554">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="24041-1555">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1555">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1556">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1556">Storage</span></span>

* <span data-ttu-id="24041-1557">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1557">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="24041-1558">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1558">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1559">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1559">VM</span></span>

* <span data-ttu-id="24041-1560">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="24041-1560">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="24041-1561">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-1561">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="24041-1562">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1562">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="24041-1563">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1563">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="24041-1564">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1564">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="24041-1565">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="24041-1565">May 7, 2018</span></span>

<span data-ttu-id="24041-1566">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="24041-1566">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="24041-1567">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1567">Core</span></span>

* <span data-ttu-id="24041-1568">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1568">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="24041-1569">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1569">Added limited support for positional arguments</span></span>
* <span data-ttu-id="24041-1570">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1570">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="24041-1571">#5591</span><span class="sxs-lookup"><span data-stu-id="24041-1571">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="24041-1572">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1572">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="24041-1573">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="24041-1573">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="24041-1574">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1574">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="24041-1575">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1575">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="24041-1576">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1576">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1577">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1577">ACR</span></span>

* <span data-ttu-id="24041-1578">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1578">Added ACR Build commands</span></span>
* <span data-ttu-id="24041-1579">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1579">Improved resource not found error messages</span></span>
* <span data-ttu-id="24041-1580">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1580">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="24041-1581">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1581">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="24041-1582">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1582">Improved repository commands error messages</span></span>
* <span data-ttu-id="24041-1583">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1583">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1584">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1584">ACS</span></span>

* <span data-ttu-id="24041-1585">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1585">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="24041-1586">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1586">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="24041-1587">AMS</span><span class="sxs-lookup"><span data-stu-id="24041-1587">AMS</span></span>

* <span data-ttu-id="24041-1588">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="24041-1588">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1589">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1589">Appservice</span></span>

* <span data-ttu-id="24041-1590">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1590">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="24041-1591">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1591">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="24041-1592">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1592">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="24041-1593">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1593">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="24041-1594">Batch AI</span><span class="sxs-lookup"><span data-stu-id="24041-1594">Batch AI</span></span>

* <span data-ttu-id="24041-1595">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1595">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="24041-1596">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="24041-1596">Cognitive Services</span></span>

* <span data-ttu-id="24041-1597">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1597">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-1598">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-1598">Consumption</span></span>

* <span data-ttu-id="24041-1599">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1599">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="24041-1600">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1600">Container</span></span>

* <span data-ttu-id="24041-1601">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1601">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="24041-1602">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="24041-1602">Cosmos DB</span></span>

* <span data-ttu-id="24041-1603">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="24041-1603">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="24041-1604">DMS</span><span class="sxs-lookup"><span data-stu-id="24041-1604">DMS</span></span>

* <span data-ttu-id="24041-1605">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1605">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1606">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1606">Extension</span></span>

* <span data-ttu-id="24041-1607">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1607">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1608">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1608">Interactive</span></span>

* <span data-ttu-id="24041-1609">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1609">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="24041-1610">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="24041-1610">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="24041-1611">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1611">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="24041-1612">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1612">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="24041-1613">랩</span><span class="sxs-lookup"><span data-stu-id="24041-1613">Lab</span></span>

* <span data-ttu-id="24041-1614">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1614">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="24041-1615">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1615">Network</span></span>

* <span data-ttu-id="24041-1616">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1616">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="24041-1617">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1617">Profile</span></span>

* <span data-ttu-id="24041-1618">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1618">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="24041-1619">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1619">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="24041-1620">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1620">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="24041-1621">Redis</span><span class="sxs-lookup"><span data-stu-id="24041-1621">Redis</span></span>

* <span data-ttu-id="24041-1622">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-1622">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="24041-1623">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1623">Deprecated `redis list-all`.</span></span> <span data-ttu-id="24041-1624">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="24041-1624">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="24041-1625">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-1625">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="24041-1626">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1626">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="24041-1627">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1627">Role</span></span>

* <span data-ttu-id="24041-1628">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1628">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1629">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1629">Storage</span></span>

* <span data-ttu-id="24041-1630">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1630">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="24041-1631">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="24041-1631">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="24041-1632">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="24041-1632">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="24041-1633">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1633">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="24041-1634">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1634">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1635">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1635">VM</span></span>

* <span data-ttu-id="24041-1636">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1636">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="24041-1637">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1637">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="24041-1638">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="24041-1638">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="24041-1639">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1639">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="24041-1640">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1640">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="24041-1641">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1641">Added write accelerator support</span></span>
* <span data-ttu-id="24041-1642">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1642">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="24041-1643">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1643">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="24041-1644">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1644">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="24041-1645">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="24041-1645">April 10, 2018</span></span>

<span data-ttu-id="24041-1646">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="24041-1646">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1647">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1647">ACR</span></span>

* <span data-ttu-id="24041-1648">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="24041-1648">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1649">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1649">ACS</span></span>

* <span data-ttu-id="24041-1650">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1650">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1651">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1651">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="24041-1653">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1653">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-1654">BatchAI</span><span class="sxs-lookup"><span data-stu-id="24041-1654">BatchAI</span></span>

* <span data-ttu-id="24041-1655">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1655">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="24041-1656">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="24041-1656">Job level mounting</span></span>
  - <span data-ttu-id="24041-1657">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="24041-1657">Environment variables with secret values</span></span>
  - <span data-ttu-id="24041-1658">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1658">Performance counters settings</span></span>
  - <span data-ttu-id="24041-1659">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="24041-1659">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="24041-1660">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="24041-1660">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="24041-1661">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="24041-1661">Usage and limits reporting</span></span>
  - <span data-ttu-id="24041-1662">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1662">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="24041-1663">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="24041-1663">Support for custom images</span></span>
  - <span data-ttu-id="24041-1664">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1664">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="24041-1665">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1665">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="24041-1666">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1666">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="24041-1667">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-1667">National clouds are supported</span></span>
* <span data-ttu-id="24041-1668">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1668">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="24041-1669">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="24041-1669">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="24041-1670">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1670">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="24041-1671">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1671">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="24041-1672">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="24041-1672">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="24041-1673">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="24041-1673">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="24041-1674">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1674">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="24041-1675">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1675">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="24041-1676">이 옵션을 사용하면 보다 쉽게 스토리지 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1676">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="24041-1677">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1677">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="24041-1678">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1678">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="24041-1679">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="24041-1679">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="24041-1680">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-1680">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="24041-1681">결제</span><span class="sxs-lookup"><span data-stu-id="24041-1681">Billing</span></span>

* <span data-ttu-id="24041-1682">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1682">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-1683">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-1683">Consumption</span></span>

* <span data-ttu-id="24041-1684">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1684">Added `marketplace` commands</span></span>
* <span data-ttu-id="24041-1685">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1685">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="24041-1686">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1686">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="24041-1687">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1687">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="24041-1688">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1688">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="24041-1689">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1689">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="24041-1690">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1690">Container</span></span>

* <span data-ttu-id="24041-1691">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="24041-1691">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="24041-1692">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="24041-1692">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1693">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1693">Extension</span></span>

* <span data-ttu-id="24041-1694">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1694">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1695">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1695">Interactive</span></span>

* <span data-ttu-id="24041-1696">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-1696">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="24041-1697">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1697">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="24041-1698">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1698">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="24041-1699">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1699">Network</span></span>

* <span data-ttu-id="24041-1700">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1700">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="24041-1701">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1701">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="24041-1702">#4910</span><span class="sxs-lookup"><span data-stu-id="24041-1702">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="24041-1703">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1703">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="24041-1704">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="24041-1704">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="24041-1705">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1705">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="24041-1706">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1706">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="24041-1707">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1707">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-1708">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1708">Profile</span></span>

* <span data-ttu-id="24041-1709">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1709">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="24041-1710">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1710">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-1711">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-1711">RDBMS</span></span>

* <span data-ttu-id="24041-1712">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1712">Added `georestore` command</span></span>
* <span data-ttu-id="24041-1713">`create` 명령에서 스토리지 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1713">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1714">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1714">Resource</span></span>

* <span data-ttu-id="24041-1715">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1715">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="24041-1716">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1716">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1717">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1717">SQL</span></span>

* <span data-ttu-id="24041-1718">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1718">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1719">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1719">Storage</span></span>

* <span data-ttu-id="24041-1720">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1720">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1721">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1721">VM</span></span>

* <span data-ttu-id="24041-1722">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1722">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="24041-1723">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-1723">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="24041-1725">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1725">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="24041-1726">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1726">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="24041-1727">#5718</span><span class="sxs-lookup"><span data-stu-id="24041-1727">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="24041-1728">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-1728">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="24041-1729">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="24041-1729">March 27, 2018</span></span>

<span data-ttu-id="24041-1730">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="24041-1730">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="24041-1731">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1731">Core</span></span>

* <span data-ttu-id="24041-1732">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="24041-1732">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1733">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1733">ACS</span></span>

* <span data-ttu-id="24041-1734">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1734">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1735">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1735">Appservice</span></span>

* <span data-ttu-id="24041-1736">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1736">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="24041-1737">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1737">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="24041-1738">Backup</span><span class="sxs-lookup"><span data-stu-id="24041-1738">Backup</span></span>

* <span data-ttu-id="24041-1739">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1739">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="24041-1740">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1740">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="24041-1741">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1741">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="24041-1742">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1742">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="24041-1743">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1743">Container</span></span>

* <span data-ttu-id="24041-1744">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1744">Added `container exec` command.</span></span> <span data-ttu-id="24041-1745">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1745">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="24041-1746">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="24041-1746">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1747">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1747">Extension</span></span>

* <span data-ttu-id="24041-1748">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1748">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="24041-1749">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1749">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="24041-1750">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1750">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1751">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1751">Interactive</span></span>

* <span data-ttu-id="24041-1752">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="24041-1752">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="24041-1753">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1753">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="24041-1754">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="24041-1754">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="24041-1755">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-1755">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="24041-1756">랩</span><span class="sxs-lookup"><span data-stu-id="24041-1756">Lab</span></span>

* <span data-ttu-id="24041-1757">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1757">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-1758">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-1758">Monitor</span></span>

* <span data-ttu-id="24041-1759">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1759">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="24041-1760">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="24041-1760">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="24041-1761">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1761">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="24041-1762">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1762">Network</span></span>

* <span data-ttu-id="24041-1763">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1763">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="24041-1764">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1764">Profile</span></span>

* <span data-ttu-id="24041-1765">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1765">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-1766">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-1766">RDBMS</span></span>

* <span data-ttu-id="24041-1767">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1767">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1768">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1768">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="24041-1770">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1770">Role</span></span>

* <span data-ttu-id="24041-1771">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1771">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="24041-1772">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1772">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="24041-1773">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1773">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="24041-1774">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1774">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="24041-1775">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1775">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1776">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1776">Storage</span></span>

* <span data-ttu-id="24041-1777">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1777">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="24041-1778">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="24041-1778">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1779">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1779">VM</span></span>

* <span data-ttu-id="24041-1780">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1780">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="24041-1781">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1781">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="24041-1782">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1782">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="24041-1783">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1783">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="24041-1784">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="24041-1784">March 13, 2018</span></span>

<span data-ttu-id="24041-1785">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="24041-1785">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1786">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1786">ACR</span></span>

* <span data-ttu-id="24041-1787">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1787">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="24041-1788">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1788">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="24041-1789">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1789">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1790">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1790">ACS</span></span>

* <span data-ttu-id="24041-1791">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1791">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="24041-1792">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1792">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="24041-1793">Advisor</span><span class="sxs-lookup"><span data-stu-id="24041-1793">Advisor</span></span>

* <span data-ttu-id="24041-1794">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1794">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="24041-1795">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1795">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="24041-1796">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1796">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="24041-1797">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1797">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="24041-1798">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1798">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1799">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1799">Appservice</span></span>

* <span data-ttu-id="24041-1800">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1800">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="24041-1801">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1801">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="24041-1802">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="24041-1802">Eventhubs</span></span>

* <span data-ttu-id="24041-1803">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1803">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1804">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1804">Extension</span></span>

* <span data-ttu-id="24041-1805">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1805">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1806">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1806">Interactive</span></span>

* <span data-ttu-id="24041-1807">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="24041-1807">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="24041-1808">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="24041-1808">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="24041-1809">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1809">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="24041-1810">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1810">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-1811">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-1811">Monitor</span></span>

* <span data-ttu-id="24041-1812">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1812">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="24041-1813">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1813">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="24041-1814">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1814">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="24041-1815">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1815">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="24041-1816">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1816">Network</span></span>

* <span data-ttu-id="24041-1817">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1817">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="24041-1818">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="24041-1818">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="24041-1819">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1819">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="24041-1820">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1820">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-1821">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1821">Profile</span></span>

* <span data-ttu-id="24041-1822">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1822">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="24041-1823">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1823">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-1824">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-1824">RDBMS</span></span>

* <span data-ttu-id="24041-1825">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1825">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="24041-1826">Service Bus</span><span class="sxs-lookup"><span data-stu-id="24041-1826">Service Bus</span></span>

* <span data-ttu-id="24041-1827">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-1827">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1828">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1828">Storage</span></span>

* <span data-ttu-id="24041-1829">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="24041-1829">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="24041-1830">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1830">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1831">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1831">VM</span></span>

* <span data-ttu-id="24041-1832">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1832">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="24041-1833">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-1833">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="24041-1834">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1834">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="24041-1835">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1835">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="24041-1836">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="24041-1836">February 27, 2018</span></span>

<span data-ttu-id="24041-1837">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="24041-1837">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="24041-1838">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1838">Core</span></span>

* <span data-ttu-id="24041-1839">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="24041-1839">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="24041-1840">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1840">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="24041-1841">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1841">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1842">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1842">ACS</span></span>

* <span data-ttu-id="24041-1843">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1843">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="24041-1844">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="24041-1844">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="24041-1845">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1845">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="24041-1846">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1846">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1847">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1847">Appservice</span></span>

* <span data-ttu-id="24041-1848">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="24041-1848">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="24041-1849">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1849">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="24041-1850">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="24041-1850">Cognitive Services</span></span>

* <span data-ttu-id="24041-1851">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1851">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-1852">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-1852">Consumption</span></span>

* <span data-ttu-id="24041-1853">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1853">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="24041-1854">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1854">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="24041-1855">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1855">Container</span></span>

* <span data-ttu-id="24041-1856">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1856">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="24041-1857">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1857">Network</span></span>

* <span data-ttu-id="24041-1858">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="24041-1858">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1859">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1859">Resource</span></span>

* <span data-ttu-id="24041-1860">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1860">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="24041-1861">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1861">Role</span></span>

* <span data-ttu-id="24041-1862">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1862">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1863">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1863">SQL</span></span>

* <span data-ttu-id="24041-1864">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1864">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1865">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1865">Storage</span></span>

* <span data-ttu-id="24041-1866">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="24041-1866">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1867">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1867">VM</span></span>

* <span data-ttu-id="24041-1868">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1868">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="24041-1869">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="24041-1869">February 13, 2018</span></span>

<span data-ttu-id="24041-1870">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="24041-1870">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="24041-1871">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1871">Core</span></span>

* <span data-ttu-id="24041-1872">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1872">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1873">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1873">ACS</span></span>

* <span data-ttu-id="24041-1874">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1874">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="24041-1875">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1875">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="24041-1876">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1876">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="24041-1877">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="24041-1877">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="24041-1878">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1878">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="24041-1879">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="24041-1879">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="24041-1880">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1880">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="24041-1881">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1881">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1882">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1882">Appservice</span></span>

* <span data-ttu-id="24041-1883">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1883">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="24041-1884">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1884">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-1885">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-1885">CDN</span></span>

* <span data-ttu-id="24041-1886">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1886">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="24041-1887">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-1887">Container</span></span>

* <span data-ttu-id="24041-1888">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1888">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="24041-1889">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1889">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-1890">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-1890">CosmosDB</span></span>

* <span data-ttu-id="24041-1891">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1891">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="24041-1892">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-1892">Extension</span></span>

* <span data-ttu-id="24041-1893">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1893">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="24041-1894">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1894">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="24041-1895">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="24041-1895">Feedback</span></span>

* <span data-ttu-id="24041-1896">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1896">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1897">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1897">Interactive</span></span>

* <span data-ttu-id="24041-1898">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1898">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="24041-1899">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1899">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="24041-1900">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-1900">IoT</span></span>

* <span data-ttu-id="24041-1901">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1901">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="24041-1902">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1902">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="24041-1903">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1903">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="24041-1904">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-1904">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-1905">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-1905">Monitor</span></span>

* <span data-ttu-id="24041-1906">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1906">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="24041-1907">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1907">Network</span></span>

* <span data-ttu-id="24041-1908">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1908">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="24041-1909">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1909">Profile</span></span>

* <span data-ttu-id="24041-1910">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="24041-1910">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1911">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1911">Resource</span></span>

* <span data-ttu-id="24041-1912">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1912">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="24041-1913">역할</span><span class="sxs-lookup"><span data-stu-id="24041-1913">Role</span></span>

* <span data-ttu-id="24041-1914">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1914">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="24041-1915">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-1915">SQL</span></span>

* <span data-ttu-id="24041-1916">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1916">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="24041-1917">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1917">Added `sql db rename`</span></span>
* <span data-ttu-id="24041-1918">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1918">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1919">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1919">Storage</span></span>

* <span data-ttu-id="24041-1920">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1920">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1921">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1921">VM</span></span>

* <span data-ttu-id="24041-1922">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1922">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="24041-1923">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1923">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="24041-1924">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="24041-1924">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="24041-1925">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="24041-1925">January 31, 2018</span></span>

<span data-ttu-id="24041-1926">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="24041-1926">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="24041-1927">코어</span><span class="sxs-lookup"><span data-stu-id="24041-1927">Core</span></span>

* <span data-ttu-id="24041-1928">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1928">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="24041-1929">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1929">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="24041-1930">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-1930">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="24041-1931">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="24041-1931">Use `--verbose` to see</span></span>
* <span data-ttu-id="24041-1932">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1932">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1933">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1933">ACS</span></span>

* <span data-ttu-id="24041-1934">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1934">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="24041-1935">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="24041-1935">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1936">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1936">Appservice</span></span>

* <span data-ttu-id="24041-1937">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="24041-1937">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="24041-1938">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="24041-1938">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-1939">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-1939">CDN</span></span>

* <span data-ttu-id="24041-1940">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1940">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-1941">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-1941">CosmosDB</span></span>

* <span data-ttu-id="24041-1942">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1942">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-1943">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-1943">Interactive</span></span>

* <span data-ttu-id="24041-1944">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1944">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="24041-1945">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-1945">Network</span></span>

* <span data-ttu-id="24041-1946">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1946">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="24041-1947">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1947">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="24041-1948">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1948">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="24041-1949">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1949">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="24041-1950">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1950">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="24041-1951">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="24041-1951">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="24041-1952">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1952">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="24041-1953">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1953">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="24041-1954">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1954">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="24041-1955">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="24041-1955">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="24041-1956">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-1956">Profile</span></span>

* <span data-ttu-id="24041-1957">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1957">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="24041-1958">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-1958">Resource</span></span>

* <span data-ttu-id="24041-1959">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1959">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="24041-1960">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-1960">Storage</span></span>

* <span data-ttu-id="24041-1961">스토리지 V1 계정을 스토리지 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-1961">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="24041-1962">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1962">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="24041-1963">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1963">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="24041-1964">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1964">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="24041-1965">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1965">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="24041-1966">VM</span><span class="sxs-lookup"><span data-stu-id="24041-1966">VM</span></span>

* <span data-ttu-id="24041-1967">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1967">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="24041-1968">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-1968">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="24041-1969">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1969">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="24041-1970">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="24041-1970">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="24041-1971">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="24041-1971">January 17, 2018</span></span>

<span data-ttu-id="24041-1972">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="24041-1972">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="24041-1973">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-1973">ACR</span></span>

* <span data-ttu-id="24041-1974">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1974">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="24041-1975">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1975">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="24041-1976">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-1976">ACS</span></span>

* <span data-ttu-id="24041-1977">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1977">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="24041-1978">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1978">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-1979">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-1979">Appservice</span></span>

* <span data-ttu-id="24041-1980">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1980">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="24041-1981">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1981">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="24041-1982">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1982">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="24041-1983">Backup</span><span class="sxs-lookup"><span data-stu-id="24041-1983">Backup</span></span>

* <span data-ttu-id="24041-1984">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1984">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="24041-1985">`backup restore restore-disks`에 스토리지 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1985">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="24041-1986">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-1986">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="24041-1987">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-1987">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="24041-1988">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1988">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="24041-1989">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-1989">Batch</span></span>

* <span data-ttu-id="24041-1990">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1990">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="24041-1991">클라우드</span><span class="sxs-lookup"><span data-stu-id="24041-1991">Cloud</span></span>

* <span data-ttu-id="24041-1992">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-1992">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-1993">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-1993">Consumption</span></span>

* <span data-ttu-id="24041-1994">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-1994">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="24041-1995">Event Grid</span><span class="sxs-lookup"><span data-stu-id="24041-1995">Event Grid</span></span>

* <span data-ttu-id="24041-1996">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="24041-1996">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="24041-1997">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="24041-1997">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="24041-1998">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-1998">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="24041-1999">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="24041-1999">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="24041-2000">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2000">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="24041-2001">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2001">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="24041-2002">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2002">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="24041-2003">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2003">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-2004">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-2004">Interactive</span></span>

* <span data-ttu-id="24041-2005">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2005">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="24041-2006">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2006">Fixed errors on startup</span></span>
* <span data-ttu-id="24041-2007">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2007">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="24041-2008">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-2008">IoT</span></span>

* <span data-ttu-id="24041-2009">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2009">Added support for device provisioning service</span></span>
* <span data-ttu-id="24041-2010">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2010">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="24041-2011">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2011">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2012">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2012">Monitor</span></span>

* <span data-ttu-id="24041-2013">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2013">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="24041-2014">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="24041-2014">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="24041-2015">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2015">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="24041-2016">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2016">Network</span></span>

* <span data-ttu-id="24041-2017">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2017">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="24041-2018">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2018">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-2019">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-2019">Profile</span></span>

* <span data-ttu-id="24041-2020">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2020">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="24041-2021">역할</span><span class="sxs-lookup"><span data-stu-id="24041-2021">Role</span></span>

* <span data-ttu-id="24041-2022">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2022">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="24041-2023">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="24041-2023">Service Fabric</span></span>

* <span data-ttu-id="24041-2024">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2024">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="24041-2025">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2025">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2026">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2026">VM</span></span>

* <span data-ttu-id="24041-2027">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2027">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="24041-2028">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2028">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="24041-2029">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2029">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="24041-2030">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2030">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="24041-2031">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2031">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="24041-2032">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2032">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="24041-2033">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2033">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="24041-2034">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2034">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="24041-2035">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="24041-2035">December 19, 2017</span></span>

<span data-ttu-id="24041-2036">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="24041-2036">Version 2.0.23</span></span>

* <span data-ttu-id="24041-2037">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2037">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="24041-2038">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-2038">Container</span></span>

* <span data-ttu-id="24041-2039">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2039">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="24041-2040">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2040">Network</span></span>

* <span data-ttu-id="24041-2041">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2041">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="24041-2042">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2042">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2043">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2043">Storage</span></span>

* <span data-ttu-id="24041-2044">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2044">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2045">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2045">VM</span></span>

* <span data-ttu-id="24041-2046">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2046">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="24041-2047">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="24041-2047">December 5, 2017</span></span>

<span data-ttu-id="24041-2048">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="24041-2048">Version 2.0.22</span></span>

* <span data-ttu-id="24041-2049">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2049">Removed `az component` commands.</span></span> <span data-ttu-id="24041-2050">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="24041-2050">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="24041-2051">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2051">Core</span></span>
* <span data-ttu-id="24041-2052">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2052">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="24041-2053">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2053">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2054">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2054">ACS</span></span>

* <span data-ttu-id="24041-2055">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2055">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="24041-2056">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-2056">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="24041-2057">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2057">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="24041-2058">Advisor</span><span class="sxs-lookup"><span data-stu-id="24041-2058">Advisor</span></span>

* <span data-ttu-id="24041-2059">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2059">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2060">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2060">Appservice</span></span>

* <span data-ttu-id="24041-2061">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2061">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="24041-2062">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2062">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="24041-2063">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2063">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="24041-2064">Consumption</span><span class="sxs-lookup"><span data-stu-id="24041-2064">Consumption</span></span>

* <span data-ttu-id="24041-2065">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2065">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="24041-2066">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-2066">Container</span></span>

* <span data-ttu-id="24041-2067">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2067">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2068">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2068">Monitor</span></span>

* <span data-ttu-id="24041-2069">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2069">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2070">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2070">Resource</span></span>

* <span data-ttu-id="24041-2071">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2071">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="24041-2072">역할</span><span class="sxs-lookup"><span data-stu-id="24041-2072">Role</span></span>

* <span data-ttu-id="24041-2073">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2073">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="24041-2074">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2074">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="24041-2075">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="24041-2075">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2076">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2076">SQL</span></span>

* <span data-ttu-id="24041-2077">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2077">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="24041-2078">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2078">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2079">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2079">VM</span></span>

* <span data-ttu-id="24041-2080">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2080">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="24041-2081">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="24041-2081">November 14, 2017</span></span>

<span data-ttu-id="24041-2082">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="24041-2082">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="24041-2083">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-2083">ACR</span></span>

* <span data-ttu-id="24041-2084">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2084">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="24041-2085">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2085">ACS</span></span>

* <span data-ttu-id="24041-2086">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2086">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="24041-2087">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="24041-2087">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="24041-2088">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2088">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="24041-2089">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2089">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="24041-2090">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2090">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2091">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2091">Appservice</span></span>

* <span data-ttu-id="24041-2092">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2092">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="24041-2093">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2093">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="24041-2094">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2094">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="24041-2095">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2095">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="24041-2096">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2096">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="24041-2097">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="24041-2097">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="24041-2098">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-2098">Batch</span></span>

* <span data-ttu-id="24041-2099">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2099">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-2100">Batchai</span><span class="sxs-lookup"><span data-stu-id="24041-2100">Batchai</span></span>

* <span data-ttu-id="24041-2101">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2101">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="24041-2102">스토리지 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2102">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="24041-2103">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2103">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="24041-2104">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2104">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="24041-2105">클라우드</span><span class="sxs-lookup"><span data-stu-id="24041-2105">Cloud</span></span>

* <span data-ttu-id="24041-2106">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2106">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="24041-2107">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-2107">Container</span></span>

* <span data-ttu-id="24041-2108">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2108">Added support to open multiple ports</span></span>
* <span data-ttu-id="24041-2109">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2109">Added container group restart policy</span></span>
* <span data-ttu-id="24041-2110">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2110">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="24041-2111">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="24041-2111">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="24041-2112">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="24041-2112">Data Lake Analytics</span></span>

* <span data-ttu-id="24041-2113">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2113">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="24041-2114">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="24041-2114">Data Lake Store</span></span>

* <span data-ttu-id="24041-2115">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2115">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="24041-2116">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-2116">Extension</span></span>

* <span data-ttu-id="24041-2117">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2117">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="24041-2118">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2118">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="24041-2119">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-2119">IoT</span></span>

* <span data-ttu-id="24041-2120">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2120">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2121">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2121">Monitor</span></span>

* <span data-ttu-id="24041-2122">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2122">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="24041-2123">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2123">Network</span></span>

* <span data-ttu-id="24041-2124">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2124">Added support for CAA DNS records</span></span>
* <span data-ttu-id="24041-2125">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2125">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="24041-2126">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2126">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="24041-2127">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2127">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="24041-2128">예약</span><span class="sxs-lookup"><span data-stu-id="24041-2128">Reservations</span></span>

* <span data-ttu-id="24041-2129">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2129">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2130">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2130">Resource</span></span>

* <span data-ttu-id="24041-2131">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2131">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2132">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2132">SQL</span></span>

* <span data-ttu-id="24041-2133">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2133">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2134">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2134">Storage</span></span>

* <span data-ttu-id="24041-2135">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2135">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="24041-2136">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2136">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="24041-2137">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2137">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="24041-2138">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="24041-2138">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="24041-2139">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2139">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="24041-2140">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2140">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="24041-2141">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2141">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2142">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2142">VM</span></span>

* <span data-ttu-id="24041-2143">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2143">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="24041-2144">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2144">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="24041-2145">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2145">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="24041-2146">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2146">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="24041-2147">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2147">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="24041-2148">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="24041-2148">October 24, 2017</span></span>

<span data-ttu-id="24041-2149">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="24041-2149">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="24041-2150">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2150">Core</span></span>

* <span data-ttu-id="24041-2151">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="24041-2151">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="24041-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-2152">ACR</span></span>

* <span data-ttu-id="24041-2153">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="24041-2153">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="24041-2154">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-2154">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="24041-2155">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="24041-2155">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2156">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2156">ACS</span></span>

* <span data-ttu-id="24041-2157">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2157">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="24041-2158">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2158">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2159">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2159">Appservice</span></span>

* <span data-ttu-id="24041-2160">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2160">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="24041-2161">구성 요소</span><span class="sxs-lookup"><span data-stu-id="24041-2161">Component</span></span>

* <span data-ttu-id="24041-2162">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2162">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2163">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2163">Monitor</span></span>

* <span data-ttu-id="24041-2164">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2164">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2165">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2165">Resource</span></span>

* <span data-ttu-id="24041-2166">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2166">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="24041-2167">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2167">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2168">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2168">VM</span></span>

* <span data-ttu-id="24041-2169">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2169">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="24041-2170">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="24041-2170">October 9, 2017</span></span>

<span data-ttu-id="24041-2171">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="24041-2171">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="24041-2172">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2172">Core</span></span>

* <span data-ttu-id="24041-2173">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2173">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2174">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2174">Appservice</span></span>

* <span data-ttu-id="24041-2175">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2175">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="24041-2176">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-2176">Batch</span></span>

* <span data-ttu-id="24041-2177">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2177">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="24041-2178">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2178">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="24041-2179">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2179">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="24041-2180">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2180">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="24041-2181">Batchai</span><span class="sxs-lookup"><span data-stu-id="24041-2181">Batchai</span></span>

* <span data-ttu-id="24041-2182">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2182">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-2183">Keyvault</span><span class="sxs-lookup"><span data-stu-id="24041-2183">Keyvault</span></span>

* <span data-ttu-id="24041-2184">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2184">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="24041-2185">(#4448)</span><span class="sxs-lookup"><span data-stu-id="24041-2185">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="24041-2186">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2186">Network</span></span>

* <span data-ttu-id="24041-2187">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2187">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="24041-2188">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2188">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2189">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2189">Resource</span></span>

* <span data-ttu-id="24041-2190">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2190">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="24041-2191">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2191">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="24041-2192">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2192">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="24041-2193">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2193">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2194">Sql</span><span class="sxs-lookup"><span data-stu-id="24041-2194">Sql</span></span>

* <span data-ttu-id="24041-2195">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2195">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="24041-2196">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2196">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="24041-2197">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2197">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2198">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2198">Storage</span></span>

* <span data-ttu-id="24041-2199">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2199">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2200">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2200">Vm</span></span>

* <span data-ttu-id="24041-2201">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2201">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="24041-2202">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2202">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="24041-2203">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2203">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="24041-2204">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2204">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="24041-2205">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2205">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="24041-2206">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="24041-2206">September 22, 2017</span></span>

<span data-ttu-id="24041-2207">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="24041-2207">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2208">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2208">Resource</span></span>

* <span data-ttu-id="24041-2209">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2209">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="24041-2210">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2210">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="24041-2211">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2211">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="24041-2212">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2212">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="24041-2213">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2213">Network</span></span>

* <span data-ttu-id="24041-2214">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2214">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="24041-2215">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2215">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="24041-2216">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2216">Added `asg` application security group commands</span></span>
* <span data-ttu-id="24041-2217">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2217">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="24041-2218">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2218">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="24041-2219">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2219">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="24041-2220">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2220">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2221">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2221">Storage</span></span>

* <span data-ttu-id="24041-2222">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2222">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="24041-2223">Event Grid</span><span class="sxs-lookup"><span data-stu-id="24041-2223">Eventgrid</span></span>

* <span data-ttu-id="24041-2224">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="24041-2224">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2225">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2225">SQL</span></span>

* <span data-ttu-id="24041-2226">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2226">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="24041-2227">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="24041-2227">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="24041-2228">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2228">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-2229">Keyvault</span><span class="sxs-lookup"><span data-stu-id="24041-2229">Keyvault</span></span>

* <span data-ttu-id="24041-2230">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2230">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2231">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2231">VM</span></span>

* <span data-ttu-id="24041-2232">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2232">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="24041-2233">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="24041-2233">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="24041-2234">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2234">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="24041-2235">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2235">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="24041-2236">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2236">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="24041-2237">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2237">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2238">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2238">ACS</span></span>

* <span data-ttu-id="24041-2239">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2239">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2240">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2240">Appservice</span></span>

* <span data-ttu-id="24041-2241">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2241">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="24041-2242">Backup</span><span class="sxs-lookup"><span data-stu-id="24041-2242">Backup</span></span>

* <span data-ttu-id="24041-2243">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2243">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="24041-2244">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="24041-2244">September 11, 2017</span></span>

<span data-ttu-id="24041-2245">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="24041-2245">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="24041-2246">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2246">Core</span></span>

* <span data-ttu-id="24041-2247">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2247">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="24041-2248">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2248">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2249">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2249">Acs</span></span>

* <span data-ttu-id="24041-2250">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2250">Added `acs list-locations` command</span></span>
* <span data-ttu-id="24041-2251">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="24041-2251">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2252">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2252">Appservice</span></span>

* <span data-ttu-id="24041-2253">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2253">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-2254">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-2254">CDN</span></span>

* <span data-ttu-id="24041-2255">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2255">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="24041-2256">내선 번호</span><span class="sxs-lookup"><span data-stu-id="24041-2256">Extension</span></span>

* <span data-ttu-id="24041-2257">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2257">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-2258">Keyvault</span><span class="sxs-lookup"><span data-stu-id="24041-2258">Keyvault</span></span>

* <span data-ttu-id="24041-2259">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2259">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="24041-2260">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2260">Network</span></span>

* <span data-ttu-id="24041-2261">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2261">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="24041-2262">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2262">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="24041-2263">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2263">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="24041-2264">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2264">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="24041-2265">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2265">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2266">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2266">Resource</span></span>

* <span data-ttu-id="24041-2267">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-2267">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="24041-2268">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-2268">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="24041-2269">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="24041-2269">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="24041-2270">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="24041-2270">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2271">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2271">SQL</span></span>

* <span data-ttu-id="24041-2272">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2272">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2273">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2273">VM</span></span>

* <span data-ttu-id="24041-2274">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2274">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="24041-2275">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="24041-2275">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="24041-2276">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2276">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="24041-2277">수정됨: `[vm|vmss] create` 스토리지 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2277">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="24041-2278">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2278">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="24041-2279">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="24041-2279">August 31, 2017</span></span>

<span data-ttu-id="24041-2280">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="24041-2280">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-2281">Keyvault</span><span class="sxs-lookup"><span data-stu-id="24041-2281">Keyvault</span></span>

* <span data-ttu-id="24041-2282">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2282">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="24041-2283">Sf</span><span class="sxs-lookup"><span data-stu-id="24041-2283">Sf</span></span>

* <span data-ttu-id="24041-2284">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2284">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2285">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2285">Storage</span></span>

* <span data-ttu-id="24041-2286">스토리지 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2286">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="24041-2287">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="24041-2287">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="24041-2288">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="24041-2288">August 28, 2017</span></span>

<span data-ttu-id="24041-2289">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="24041-2289">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="24041-2290">CLI</span><span class="sxs-lookup"><span data-stu-id="24041-2290">CLI</span></span>

* <span data-ttu-id="24041-2291">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2291">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2292">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2292">ACS</span></span>

* <span data-ttu-id="24041-2293">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2293">Corrected preview regions</span></span>
* <span data-ttu-id="24041-2294">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2294">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="24041-2295">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="24041-2295">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2296">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2296">Appservice</span></span>

* <span data-ttu-id="24041-2297">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2297">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="24041-2298">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2298">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="24041-2299">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2299">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="24041-2300">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2300">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="24041-2301">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="24041-2301">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="24041-2302">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-2302">IoT</span></span>

* <span data-ttu-id="24041-2303">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2303">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="24041-2304">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2304">Network</span></span>

* <span data-ttu-id="24041-2305">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2305">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="24041-2306">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2306">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="24041-2307">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2307">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="24041-2308">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2308">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="24041-2309">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2309">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-2310">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-2310">Profile</span></span>

* <span data-ttu-id="24041-2311">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2311">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="24041-2312">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="24041-2312">Service Fabric</span></span>

* <span data-ttu-id="24041-2313">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2313">Preview release</span></span>
* <span data-ttu-id="24041-2314">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="24041-2314">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="24041-2315">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2315">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="24041-2316">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2316">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2317">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2317">Storage</span></span>

* <span data-ttu-id="24041-2318">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2318">Enabled setting blob tier</span></span>
* <span data-ttu-id="24041-2319">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2319">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="24041-2320">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2320">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="24041-2321">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2321">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="24041-2322">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2322">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="24041-2323">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2323">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2324">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2324">VM</span></span>

* <span data-ttu-id="24041-2325">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2325">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="24041-2326">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2326">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="24041-2327">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2327">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="24041-2328">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2328">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="24041-2329">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2329">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="24041-2330">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2330">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="24041-2331">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="24041-2331">August 15, 2017</span></span>

<span data-ttu-id="24041-2332">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="24041-2332">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2333">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2333">ACS</span></span>

* <span data-ttu-id="24041-2334">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2334">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2335">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2335">Appservice</span></span>

* <span data-ttu-id="24041-2336">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2336">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="24041-2337">Event Grid</span><span class="sxs-lookup"><span data-stu-id="24041-2337">Event Grid</span></span>

* <span data-ttu-id="24041-2338">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2338">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="24041-2339">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="24041-2339">August 11, 2017</span></span>

<span data-ttu-id="24041-2340">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="24041-2340">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2341">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2341">ACS</span></span>

* <span data-ttu-id="24041-2342">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2342">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="24041-2343">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-2343">Batch</span></span>

* <span data-ttu-id="24041-2344">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2344">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="24041-2345">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2345">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="24041-2346">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2346">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="24041-2347">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2347">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="24041-2348">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2348">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="24041-2349">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2349">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="24041-2350">구성 요소</span><span class="sxs-lookup"><span data-stu-id="24041-2350">Component</span></span>

* <span data-ttu-id="24041-2351">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2351">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="24041-2352">컨테이너</span><span class="sxs-lookup"><span data-stu-id="24041-2352">Container</span></span>

* <span data-ttu-id="24041-2353">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2353">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="24041-2354">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="24041-2354">Data Lake Store</span></span>

* <span data-ttu-id="24041-2355">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2355">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="24041-2356">Event Grid</span><span class="sxs-lookup"><span data-stu-id="24041-2356">Event Grid</span></span>

* <span data-ttu-id="24041-2357">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2357">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="24041-2358">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2358">Network</span></span>

* <span data-ttu-id="24041-2359">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2359">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="24041-2360">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2360">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="24041-2361">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2361">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="24041-2362">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2362">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="24041-2363">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-2363">Profile</span></span>

* <span data-ttu-id="24041-2364">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2364">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2365">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2365">Storage</span></span>

* <span data-ttu-id="24041-2366">시스템에 할당된 ID를 통한 스토리지 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2366">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2367">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2367">VM</span></span>

* <span data-ttu-id="24041-2368">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2368">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="24041-2369">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2369">Exposed `list-skus` command</span></span>
* <span data-ttu-id="24041-2370">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2370">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="24041-2371">데이터 디스크 연결 시 스토리지 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2371">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="24041-2372">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 스토리지 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2372">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="24041-2373">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="24041-2373">July 28, 2017</span></span>

<span data-ttu-id="24041-2374">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="24041-2374">Version 2.0.12</span></span>

* <span data-ttu-id="24041-2375">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2375">Added container commands</span></span>
* <span data-ttu-id="24041-2376">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2376">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="24041-2377">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2377">Core</span></span>

* <span data-ttu-id="24041-2378">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="24041-2378">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="24041-2379">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="24041-2379">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="24041-2380">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-2380">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="24041-2381">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="24041-2381">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="24041-2382">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="24041-2382">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="24041-2383">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="24041-2383">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="24041-2384">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="24041-2384">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="24041-2385">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="24041-2385">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="24041-2386">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="24041-2386">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="24041-2387">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="24041-2387">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="24041-2388">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="24041-2388">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="24041-2389">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="24041-2389">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="24041-2390">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2390">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="24041-2391">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2391">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="24041-2392">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2392">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="24041-2393">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="24041-2393">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="24041-2394">ACR</span><span class="sxs-lookup"><span data-stu-id="24041-2394">ACR</span></span>

* <span data-ttu-id="24041-2395">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2395">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="24041-2396">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2396">Support SKU update for managed registries</span></span>
* <span data-ttu-id="24041-2397">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2397">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="24041-2398">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2398">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="24041-2399">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2399">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="24041-2400">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2400">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2401">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2401">ACS</span></span>

* <span data-ttu-id="24041-2402">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2402">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2403">App Service</span><span class="sxs-lookup"><span data-stu-id="24041-2403">Appservice</span></span>

* <span data-ttu-id="24041-2404">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2404">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="24041-2405">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2405">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="24041-2406">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2406">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="24041-2407">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="24041-2407">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="24041-2408">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="24041-2408">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="24041-2409">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="24041-2409">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="24041-2410">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="24041-2410">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="24041-2411">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="24041-2411">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="24041-2412">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2412">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="24041-2413">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2413">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="24041-2414">Batch</span><span class="sxs-lookup"><span data-stu-id="24041-2414">Batch</span></span>

* <span data-ttu-id="24041-2415">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2415">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="24041-2416">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2416">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="24041-2417">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2417">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="24041-2418">CDN</span><span class="sxs-lookup"><span data-stu-id="24041-2418">CDN</span></span>

* <span data-ttu-id="24041-2419">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="24041-2419">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="24041-2420">클라우드</span><span class="sxs-lookup"><span data-stu-id="24041-2420">Cloud</span></span>

* <span data-ttu-id="24041-2421">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2421">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="24041-2422">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2422">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="24041-2423">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2423">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="24041-2424">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="24041-2424">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="24041-2425">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="24041-2425">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-2426">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-2426">CosmosDB</span></span>

* <span data-ttu-id="24041-2427">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2427">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="24041-2428">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2428">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="24041-2429">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="24041-2429">Data Lake Analytics</span></span>

* <span data-ttu-id="24041-2430">`dla account compute-policy` 제목 아래에 컴퓨팅 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2430">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="24041-2431">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2431">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="24041-2432">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2432">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="24041-2433">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="24041-2433">Data Lake Store</span></span>

* <span data-ttu-id="24041-2434">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2434">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="24041-2435">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2435">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="24041-2436">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2436">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="24041-2437">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="24041-2437">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="24041-2438">대화형</span><span class="sxs-lookup"><span data-stu-id="24041-2438">Interactive</span></span>

* <span data-ttu-id="24041-2439">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2439">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="24041-2440">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2440">Increased test coverage</span></span>
* <span data-ttu-id="24041-2441">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2441">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="24041-2442">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="24041-2442">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="24041-2443">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="24041-2443">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="24041-2444">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="24041-2444">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="24041-2445">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="24041-2445">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="24041-2446">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2446">Added `--progress` flag</span></span>
* <span data-ttu-id="24041-2447">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2447">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="24041-2448">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="24041-2448">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="24041-2449">IoT</span><span class="sxs-lookup"><span data-stu-id="24041-2449">IoT</span></span>

* <span data-ttu-id="24041-2450">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2450">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="24041-2451">(#3934)</span><span class="sxs-lookup"><span data-stu-id="24041-2451">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="24041-2452">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="24041-2452">Key vault</span></span>

* <span data-ttu-id="24041-2453">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="24041-2453">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="24041-2454">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="24041-2454">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="24041-2455">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="24041-2455">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="24041-2456">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="24041-2456">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="24041-2457">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="24041-2457">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="24041-2458">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="24041-2458">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="24041-2459">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="24041-2459">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="24041-2460">(#3307)</span><span class="sxs-lookup"><span data-stu-id="24041-2460">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="24041-2461">랩</span><span class="sxs-lookup"><span data-stu-id="24041-2461">Lab</span></span>

* <span data-ttu-id="24041-2462">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2462">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="24041-2463">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2463">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2464">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2464">Monitor</span></span>

* <span data-ttu-id="24041-2465">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="24041-2465">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="24041-2466">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2466">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="24041-2467">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2467">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="24041-2468">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2468">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="24041-2469">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="24041-2469">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="24041-2470">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="24041-2470">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="24041-2471">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2471">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="24041-2472">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2472">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="24041-2473">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2473">`location` no longer required</span></span>
  * <span data-ttu-id="24041-2474">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2474">Add name and ID support for target</span></span>
  * <span data-ttu-id="24041-2475">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2475">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="24041-2476">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2476">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="24041-2477">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2477">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="24041-2478">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2478">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="24041-2479">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2479">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="24041-2480">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2480">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="24041-2481">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2481">Network</span></span>

* <span data-ttu-id="24041-2482">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2482">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="24041-2483">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2483">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="24041-2484">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2484">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="24041-2485">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2485">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="24041-2486">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2486">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="24041-2487">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2487">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="24041-2488">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="24041-2488">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="24041-2489">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="24041-2489">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="24041-2490">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="24041-2490">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="24041-2491">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="24041-2491">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="24041-2492">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="24041-2492">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="24041-2493">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="24041-2493">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="24041-2494">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="24041-2494">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="24041-2495">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="24041-2495">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="24041-2496">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2496">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="24041-2497">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2497">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="24041-2498">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2498">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="24041-2499">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2499">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="24041-2500">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2500">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="24041-2501">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2501">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="24041-2502">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2502">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="24041-2503">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2503">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="24041-2504">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2504">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="24041-2505">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2505">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="24041-2506">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2506">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="24041-2507">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2507">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="24041-2508">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="24041-2508">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="24041-2509">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-2509">Profile</span></span>

* <span data-ttu-id="24041-2510">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2510">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="24041-2511">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2511">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="24041-2512">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="24041-2512">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="24041-2513">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2513">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="24041-2514">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2514">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="24041-2515">RDBMS</span><span class="sxs-lookup"><span data-stu-id="24041-2515">RDBMS</span></span>

* <span data-ttu-id="24041-2516">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="24041-2516">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="24041-2517">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="24041-2517">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="24041-2518">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="24041-2518">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="24041-2519">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="24041-2519">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2520">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2520">Resource</span></span>

* <span data-ttu-id="24041-2521">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2521">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="24041-2522">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="24041-2522">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="24041-2523">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2523">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="24041-2524">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2524">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="24041-2525">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="24041-2525">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="24041-2526">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2526">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="24041-2527">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="24041-2527">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="24041-2528">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2528">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="24041-2529">역할</span><span class="sxs-lookup"><span data-stu-id="24041-2529">Role</span></span>

* <span data-ttu-id="24041-2530">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2530">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="24041-2531">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="24041-2531">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="24041-2532">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="24041-2532">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="24041-2533">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="24041-2533">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="24041-2534">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2534">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="24041-2535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="24041-2535">Service Fabric</span></span>
* <span data-ttu-id="24041-2536">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="24041-2536">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="24041-2537">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="24041-2537">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="24041-2538">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="24041-2538">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2539">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2539">SQL</span></span>

* <span data-ttu-id="24041-2540">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2540">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="24041-2541">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="24041-2541">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="24041-2542">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2542">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2543">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2543">Storage</span></span>

* <span data-ttu-id="24041-2544">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="24041-2544">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="24041-2545">HTTPS 전용 스토리지 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="24041-2545">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="24041-2546">스토리지 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="24041-2546">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="24041-2547">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2547">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="24041-2548">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="24041-2548">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="24041-2549">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="24041-2549">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2550">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2550">VM</span></span>

* <span data-ttu-id="24041-2551">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2551">Support configuring nsg</span></span>
* <span data-ttu-id="24041-2552">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2552">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="24041-2553">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="24041-2553">Support managed service identities</span></span>
* <span data-ttu-id="24041-2554">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="24041-2554">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="24041-2555">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="24041-2555">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="24041-2556">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="24041-2556">May 10, 2017</span></span>

<span data-ttu-id="24041-2557">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="24041-2557">Version 2.0.6</span></span>

* <span data-ttu-id="24041-2558">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="24041-2558">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="24041-2559">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2559">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="24041-2560">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="24041-2560">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="24041-2561">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="24041-2561">Include Cognitive Services module</span></span>
* <span data-ttu-id="24041-2562">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="24041-2562">Include Service Fabric module</span></span>
* <span data-ttu-id="24041-2563">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="24041-2563">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="24041-2564">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2564">Add support for CDN commands</span></span>
* <span data-ttu-id="24041-2565">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="24041-2565">Remove Container module</span></span>
* <span data-ttu-id="24041-2566">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="24041-2566">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="24041-2567">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="24041-2567">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="24041-2568">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2568">Core</span></span>

* <span data-ttu-id="24041-2569">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="24041-2569">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="24041-2570">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="24041-2570">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="24041-2571">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="24041-2571">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="24041-2572">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="24041-2572">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="24041-2573">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="24041-2573">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="24041-2574">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="24041-2574">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="24041-2575">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="24041-2575">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="24041-2576">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="24041-2576">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="24041-2577">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="24041-2577">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="24041-2578">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="24041-2578">core: Improved performance</span></span>
* <span data-ttu-id="24041-2579">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2579">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="24041-2580">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="24041-2580">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2581">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2581">ACS</span></span>

* <span data-ttu-id="24041-2582">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2582">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="24041-2583">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="24041-2583">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="24041-2584">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="24041-2584">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="24041-2585">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="24041-2585">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2586">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-2586">AppService</span></span>

* <span data-ttu-id="24041-2587">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="24041-2587">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="24041-2588">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2588">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="24041-2589">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="24041-2589">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="24041-2590">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="24041-2590">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="24041-2591">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="24041-2591">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="24041-2592">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="24041-2592">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="24041-2593">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2593">support slot swap with preview</span></span>
* <span data-ttu-id="24041-2594">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="24041-2594">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="24041-2595">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="24041-2595">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="24041-2596">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="24041-2596">CosmosDB</span></span>

* <span data-ttu-id="24041-2597">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="24041-2597">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="24041-2598">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2598">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="24041-2599">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2599">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="24041-2600">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2600">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="24041-2601">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="24041-2601">Data Lake Analytics</span></span>

* <span data-ttu-id="24041-2602">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2602">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="24041-2603">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2603">Add support for new catalog item type: package.</span></span> <span data-ttu-id="24041-2604">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="24041-2604">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="24041-2605">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="24041-2605">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="24041-2606">테이블</span><span class="sxs-lookup"><span data-stu-id="24041-2606">Table</span></span>
  * <span data-ttu-id="24041-2607">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="24041-2607">Table valued function</span></span>
  * <span data-ttu-id="24041-2608">보기</span><span class="sxs-lookup"><span data-stu-id="24041-2608">View</span></span>
  * <span data-ttu-id="24041-2609">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="24041-2609">Table Statistics.</span></span> <span data-ttu-id="24041-2610">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="24041-2610">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="24041-2611">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="24041-2611">Data Lake Store</span></span>

* <span data-ttu-id="24041-2612">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="24041-2612">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="24041-2613">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="24041-2613">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="24041-2614">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="24041-2614">missed help for access show.</span></span> <span data-ttu-id="24041-2615">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2615">adding it.</span></span> <span data-ttu-id="24041-2616">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="24041-2616">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="24041-2617">찾기</span><span class="sxs-lookup"><span data-stu-id="24041-2617">Find</span></span>

* <span data-ttu-id="24041-2618">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="24041-2618">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="24041-2619">KeyVault</span><span class="sxs-lookup"><span data-stu-id="24041-2619">KeyVault</span></span>

* <span data-ttu-id="24041-2620">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2620">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="24041-2621">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="24041-2621">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="24041-2622">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2622">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="24041-2623">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2623">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="24041-2624">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="24041-2624">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="24041-2625">랩</span><span class="sxs-lookup"><span data-stu-id="24041-2625">Lab</span></span>

* <span data-ttu-id="24041-2626">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2626">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="24041-2627">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2627">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="24041-2628">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="24041-2628">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="24041-2629">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="24041-2629">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="24041-2630">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2630">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="24041-2631">모니터</span><span class="sxs-lookup"><span data-stu-id="24041-2631">Monitor</span></span>

* <span data-ttu-id="24041-2632">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="24041-2632">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="24041-2633">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="24041-2633">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="24041-2634">네트워크</span><span class="sxs-lookup"><span data-stu-id="24041-2634">Network</span></span>

* <span data-ttu-id="24041-2635">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2635">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="24041-2636">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2636">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="24041-2637">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2637">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="24041-2638">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2638">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="24041-2639">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2639">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="24041-2640">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2640">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="24041-2641">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2641">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="24041-2642">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2642">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="24041-2643">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2643">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="24041-2644">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2644">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="24041-2645">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="24041-2645">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="24041-2646">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2646">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="24041-2647">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2647">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="24041-2648">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2648">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="24041-2649">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="24041-2649">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="24041-2650">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2650">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="24041-2651">프로필</span><span class="sxs-lookup"><span data-stu-id="24041-2651">Profile</span></span>

* <span data-ttu-id="24041-2652">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="24041-2652">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="24041-2653">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="24041-2653">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="24041-2654">Redis</span><span class="sxs-lookup"><span data-stu-id="24041-2654">Redis</span></span>

* <span data-ttu-id="24041-2655">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2655">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="24041-2656">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="24041-2656">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="24041-2657">리소스</span><span class="sxs-lookup"><span data-stu-id="24041-2657">Resource</span></span>

* <span data-ttu-id="24041-2658">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="24041-2658">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="24041-2659">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="24041-2659">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="24041-2660">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="24041-2660">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="24041-2661">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2661">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="24041-2662">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="24041-2662">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="24041-2663">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2663">Add docs for az lock update.</span></span> <span data-ttu-id="24041-2664">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="24041-2664">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="24041-2665">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2665">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="24041-2666">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="24041-2666">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="24041-2667">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2667">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="24041-2668">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="24041-2668">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="24041-2669">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="24041-2669">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="24041-2670">역할</span><span class="sxs-lookup"><span data-stu-id="24041-2670">Role</span></span>

* <span data-ttu-id="24041-2671">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="24041-2671">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="24041-2672">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="24041-2672">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="24041-2673">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="24041-2673">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="24041-2674">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="24041-2674">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="24041-2675">SQL</span><span class="sxs-lookup"><span data-stu-id="24041-2675">SQL</span></span>

* <span data-ttu-id="24041-2676">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="24041-2676">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="24041-2677">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="24041-2677">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="24041-2678">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2678">Storage</span></span>

* <span data-ttu-id="24041-2679">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="24041-2679">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="24041-2680">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2680">Add support for incremental blob copy</span></span>
* <span data-ttu-id="24041-2681">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2681">Add support for large block blob upload</span></span>
* <span data-ttu-id="24041-2682">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="24041-2682">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2683">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2683">VM</span></span>

* <span data-ttu-id="24041-2684">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="24041-2684">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="24041-2685">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="24041-2685">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="24041-2686">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="24041-2686">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="24041-2687">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="24041-2687">az vm/vmss disk</span></span>
  3. <span data-ttu-id="24041-2688">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2688">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="24041-2689">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="24041-2689">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="24041-2690">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="24041-2690">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="24041-2691">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="24041-2691">April 3, 2017</span></span>

<span data-ttu-id="24041-2692">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="24041-2692">Version 2.0.2</span></span>

<span data-ttu-id="24041-2693">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2693">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="24041-2694">코어</span><span class="sxs-lookup"><span data-stu-id="24041-2694">Core</span></span>

* <span data-ttu-id="24041-2695">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="24041-2695">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="24041-2696">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="24041-2696">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="24041-2697">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="24041-2697">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="24041-2698">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="24041-2698">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="24041-2699">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="24041-2699">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="24041-2700">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="24041-2700">Add prompting for missing template parameters.</span></span> <span data-ttu-id="24041-2701">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="24041-2701">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="24041-2702">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2702">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="24041-2703">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="24041-2703">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="24041-2704">ACS</span><span class="sxs-lookup"><span data-stu-id="24041-2704">ACS</span></span>

* <span data-ttu-id="24041-2705">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="24041-2705">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="24041-2706">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="24041-2706">Add support for ssh key password prompting.</span></span> <span data-ttu-id="24041-2707">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="24041-2707">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="24041-2708">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="24041-2708">Add support for windows clusters.</span></span> <span data-ttu-id="24041-2709">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="24041-2709">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="24041-2710">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="24041-2710">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="24041-2711">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="24041-2711">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="24041-2712">AppService</span><span class="sxs-lookup"><span data-stu-id="24041-2712">AppService</span></span>

* <span data-ttu-id="24041-2713">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="24041-2713">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="24041-2714">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="24041-2714">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="24041-2715">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="24041-2715">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="24041-2716">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="24041-2716">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="24041-2717">DataLake</span><span class="sxs-lookup"><span data-stu-id="24041-2717">DataLake</span></span>

* <span data-ttu-id="24041-2718">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2718">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="24041-2719">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="24041-2719">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="24041-2720">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="24041-2720">DocuemntDB</span></span>

* <span data-ttu-id="24041-2721">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="24041-2721">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="24041-2722">VM</span><span class="sxs-lookup"><span data-stu-id="24041-2722">VM</span></span>

* <span data-ttu-id="24041-2723">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="24041-2723">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="24041-2724">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="24041-2724">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="24041-2725">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="24041-2725">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="24041-2726">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="24041-2726">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="24041-2727">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="24041-2727">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="24041-2728">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="24041-2728">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="24041-2729">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="24041-2729">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="24041-2730">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="24041-2730">February 27, 2017</span></span>

<span data-ttu-id="24041-2731">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="24041-2731">Version 2.0.0</span></span>

<span data-ttu-id="24041-2732">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2732">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="24041-2733">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="24041-2733">Container Service (acs)</span></span>
- <span data-ttu-id="24041-2734">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="24041-2734">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="24041-2735">네트워킹</span><span class="sxs-lookup"><span data-stu-id="24041-2735">Networking</span></span>
- <span data-ttu-id="24041-2736">스토리지</span><span class="sxs-lookup"><span data-stu-id="24041-2736">Storage</span></span>

<span data-ttu-id="24041-2737">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2737">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="24041-2738">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2738">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="24041-2739">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2739">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="24041-2740">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2740">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="24041-2741">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="24041-2741">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="24041-2742">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="24041-2742">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="24041-2743">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="24041-2743">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="24041-2744">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="24041-2744">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="24041-2745">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="24041-2745">Provide feedback from the command line with the `az feedback` command</span></span>


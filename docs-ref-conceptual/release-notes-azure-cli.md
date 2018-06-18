---
title: Azure CLI 2.0 릴리스 정보
description: Azure CLI 2.0 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 72e667d74ff8d55f26ecbf3b3c8845c9c03b56be
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512906"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="4b951-103">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="4b951-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4b951-104">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="4b951-104">June 13, 2018</span></span>

<span data-ttu-id="4b951-105">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4b951-105">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4b951-106">AKS</span><span class="sxs-lookup"><span data-stu-id="4b951-106">AKS</span></span>

* <span data-ttu-id="4b951-107">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-107">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4b951-108">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="4b951-108">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="4b951-109">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-109">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4b951-110">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-110">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4b951-111">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-111">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-112">AppService</span><span class="sxs-lookup"><span data-stu-id="4b951-112">AppService</span></span>

* <span data-ttu-id="4b951-113">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-113">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b951-114">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="4b951-114">June 5, 2018</span></span>

<span data-ttu-id="4b951-115">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4b951-115">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-116">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-116">Interactive</span></span>

* <span data-ttu-id="4b951-117">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="4b951-117">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b951-118">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="4b951-118">June 5, 2018</span></span>

<span data-ttu-id="4b951-119">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4b951-119">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4b951-120">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-120">Core</span></span>

* <span data-ttu-id="4b951-121">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-121">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4b951-122">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-122">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-123">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-123">ACR</span></span>

* <span data-ttu-id="4b951-124">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-124">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4b951-125">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-125">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4b951-126">AKS</span><span class="sxs-lookup"><span data-stu-id="4b951-126">AKS</span></span>

* <span data-ttu-id="4b951-127">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-127">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-128">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-128">Batch</span></span>

* <span data-ttu-id="4b951-129">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4b951-129">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-130">IOT</span><span class="sxs-lookup"><span data-stu-id="4b951-130">IOT</span></span>

* <span data-ttu-id="4b951-131">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-131">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4b951-132">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-132">Network</span></span>

* <span data-ttu-id="4b951-133">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="4b951-133">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4b951-134">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="4b951-134">Policy Insights</span></span>

* <span data-ttu-id="4b951-135">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-135">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4b951-136">ARM</span><span class="sxs-lookup"><span data-stu-id="4b951-136">ARM</span></span>

* <span data-ttu-id="4b951-137">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-137">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-138">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-138">SQL</span></span>

* <span data-ttu-id="4b951-139">관리형 새 인스턴스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-139">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4b951-140">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-140">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4b951-141">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-141">Storage</span></span>

* <span data-ttu-id="4b951-142">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="4b951-142">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-143">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-143">VM</span></span>

* <span data-ttu-id="4b951-144">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-144">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4b951-145">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-145">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4b951-146">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-146">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4b951-147">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="4b951-147">May 22, 2018</span></span>

<span data-ttu-id="4b951-148">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4b951-148">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4b951-149">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-149">Core</span></span>

* <span data-ttu-id="4b951-150">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-150">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-151">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-151">ACS</span></span>

* <span data-ttu-id="4b951-152">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-152">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4b951-153">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-153">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-154">AppService</span><span class="sxs-lookup"><span data-stu-id="4b951-154">AppService</span></span>

* <span data-ttu-id="4b951-155">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-155">Improved generic update commands</span></span>
* <span data-ttu-id="4b951-156">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-156">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4b951-157">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-157">Container</span></span>

* <span data-ttu-id="4b951-158">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-158">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4b951-159">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-159">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-160">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-160">Extension</span></span>

* <span data-ttu-id="4b951-161">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-161">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-162">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-162">Interactive</span></span>

* <span data-ttu-id="4b951-163">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-163">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4b951-164">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="4b951-164">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-165">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b951-165">KeyVault</span></span>

* <span data-ttu-id="4b951-166">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="4b951-166">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4b951-167">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-167">Network</span></span>

* <span data-ttu-id="4b951-168">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="4b951-168">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4b951-169">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-169">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-170">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-170">SQL</span></span>

* <span data-ttu-id="4b951-171">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="4b951-171">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4b951-172">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="4b951-172">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4b951-173">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-173">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="4b951-174">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-174">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4b951-175">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-175">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4b951-176">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="4b951-176">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4b951-177">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="4b951-177">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4b951-178">`edition`</span><span class="sxs-lookup"><span data-stu-id="4b951-178">`edition`.</span></span> <span data-ttu-id="4b951-179">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="4b951-179">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4b951-180">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="4b951-180">`elasticPoolName`.</span></span> <span data-ttu-id="4b951-181">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="4b951-181">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4b951-182">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-182">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4b951-183">`edition`</span><span class="sxs-lookup"><span data-stu-id="4b951-183">`edition`.</span></span> <span data-ttu-id="4b951-184">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="4b951-184">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4b951-185">`dtu`</span><span class="sxs-lookup"><span data-stu-id="4b951-185">`dtu`.</span></span> <span data-ttu-id="4b951-186">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="4b951-186">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4b951-187">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="4b951-187">`databaseDtuMin`.</span></span> <span data-ttu-id="4b951-188">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="4b951-188">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4b951-189">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="4b951-189">`databaseDtuMax`.</span></span> <span data-ttu-id="4b951-190">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="4b951-190">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4b951-191">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-191">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4b951-192">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-192">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-193">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-193">Storage</span></span>

* <span data-ttu-id="4b951-194">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-194">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4b951-195">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-195">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-196">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-196">VM</span></span>

* <span data-ttu-id="4b951-197">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="4b951-197">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4b951-198">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="4b951-198">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4b951-199">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="4b951-199">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4b951-200">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="4b951-200">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4b951-201">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-201">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4b951-202">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="4b951-202">May 7, 2018</span></span>

<span data-ttu-id="4b951-203">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4b951-203">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4b951-204">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-204">Core</span></span>

* <span data-ttu-id="4b951-205">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-205">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4b951-206">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-206">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4b951-207">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-207">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4b951-208">#5591</span><span class="sxs-lookup"><span data-stu-id="4b951-208">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4b951-209">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-209">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4b951-210">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-210">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4b951-211">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-211">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4b951-212">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-212">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4b951-213">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-213">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-214">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-214">ACR</span></span>

* <span data-ttu-id="4b951-215">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-215">Added ACR Build commands</span></span>
* <span data-ttu-id="4b951-216">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-216">Improved resource not found error messages</span></span>
* <span data-ttu-id="4b951-217">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-217">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4b951-218">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-218">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4b951-219">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-219">Improved repository commands error messages</span></span>
* <span data-ttu-id="4b951-220">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="4b951-220">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-221">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-221">ACS</span></span>

* <span data-ttu-id="4b951-222">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-222">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4b951-223">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-223">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4b951-224">AMS</span><span class="sxs-lookup"><span data-stu-id="4b951-224">AMS</span></span>

* <span data-ttu-id="4b951-225">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="4b951-225">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-226">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-226">Appservice</span></span>

* <span data-ttu-id="4b951-227">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-227">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4b951-228">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-228">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4b951-229">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-229">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4b951-230">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-230">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b951-231">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b951-231">Batch AI</span></span>

* <span data-ttu-id="4b951-232">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-232">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b951-233">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b951-233">Cognitive Services</span></span>

* <span data-ttu-id="4b951-234">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-234">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4b951-235">Consumption</span><span class="sxs-lookup"><span data-stu-id="4b951-235">Consumption</span></span>

* <span data-ttu-id="4b951-236">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-236">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4b951-237">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-237">Container</span></span>

* <span data-ttu-id="4b951-238">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-238">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4b951-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b951-239">Cosmos DB</span></span>

* <span data-ttu-id="4b951-240">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b951-240">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4b951-241">DMS</span><span class="sxs-lookup"><span data-stu-id="4b951-241">DMS</span></span>

* <span data-ttu-id="4b951-242">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-242">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-243">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-243">Extension</span></span>

* <span data-ttu-id="4b951-244">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-244">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-245">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-245">Interactive</span></span>

* <span data-ttu-id="4b951-246">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-246">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4b951-247">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="4b951-247">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4b951-248">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-248">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4b951-249">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-249">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4b951-250">랩</span><span class="sxs-lookup"><span data-stu-id="4b951-250">Lab</span></span>

* <span data-ttu-id="4b951-251">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-251">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4b951-252">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-252">Network</span></span>

* <span data-ttu-id="4b951-253">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-253">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4b951-254">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-254">Profile</span></span>

* <span data-ttu-id="4b951-255">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-255">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4b951-256">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-256">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4b951-257">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-257">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4b951-258">Redis</span><span class="sxs-lookup"><span data-stu-id="4b951-258">Redis</span></span>

* <span data-ttu-id="4b951-259">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-259">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4b951-260">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-260">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4b951-261">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="4b951-261">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4b951-262">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-262">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4b951-263">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-263">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4b951-264">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-264">Role</span></span>

* <span data-ttu-id="4b951-265">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-265">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-266">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-266">Storage</span></span>

* <span data-ttu-id="4b951-267">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-267">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4b951-268">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="4b951-268">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4b951-269">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="4b951-269">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4b951-270">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-270">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4b951-271">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-271">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-272">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-272">VM</span></span>

* <span data-ttu-id="4b951-273">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-273">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4b951-274">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-274">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4b951-275">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="4b951-275">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4b951-276">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-276">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4b951-277">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-277">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4b951-278">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-278">Added write accelerator support</span></span> 
* <span data-ttu-id="4b951-279">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-279">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4b951-280">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-280">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4b951-281">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-281">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4b951-282">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="4b951-282">April 10, 2018</span></span>

<span data-ttu-id="4b951-283">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4b951-283">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-284">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-284">ACR</span></span>

* <span data-ttu-id="4b951-285">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="4b951-285">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-286">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-286">ACS</span></span>

* <span data-ttu-id="4b951-287">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-287">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-288">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-288">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4b951-290">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-290">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4b951-291">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b951-291">BatchAI</span></span>

* <span data-ttu-id="4b951-292">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-292">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="4b951-293">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="4b951-293">Job level mounting</span></span>
 - <span data-ttu-id="4b951-294">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="4b951-294">Environment variables with secret values</span></span>
 - <span data-ttu-id="4b951-295">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="4b951-295">Performance counters settings</span></span>
 - <span data-ttu-id="4b951-296">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="4b951-296">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="4b951-297">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-297">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="4b951-298">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="4b951-298">Usage and limits reporting</span></span>
 - <span data-ttu-id="4b951-299">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-299">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="4b951-300">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-300">Support for custom images</span></span>
 - <span data-ttu-id="4b951-301">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-301">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4b951-302">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-302">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4b951-303">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-303">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4b951-304">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-304">National clouds are supported</span></span>
* <span data-ttu-id="4b951-305">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-305">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4b951-306">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="4b951-306">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4b951-307">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-307">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4b951-308">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-308">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4b951-309">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="4b951-309">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4b951-310">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="4b951-310">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4b951-311">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-311">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4b951-312">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-312">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4b951-313">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-313">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4b951-314">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-314">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4b951-315">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-315">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4b951-316">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="4b951-316">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4b951-317">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-317">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4b951-318">결제</span><span class="sxs-lookup"><span data-stu-id="4b951-318">Billing</span></span>

* <span data-ttu-id="4b951-319">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-319">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4b951-320">Consumption</span><span class="sxs-lookup"><span data-stu-id="4b951-320">Consumption</span></span>

* <span data-ttu-id="4b951-321">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-321">Added `marketplace` commands</span></span>
* <span data-ttu-id="4b951-322">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-322">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4b951-323">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-323">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4b951-324">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-324">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4b951-325">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-325">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4b951-326">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-326">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b951-327">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-327">Container</span></span>

* <span data-ttu-id="4b951-328">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="4b951-328">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4b951-329">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="4b951-329">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-330">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-330">Extension</span></span>

* <span data-ttu-id="4b951-331">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-331">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-332">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-332">Interactive</span></span>

* <span data-ttu-id="4b951-333">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-333">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4b951-334">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-334">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4b951-335">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-335">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4b951-336">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-336">Network</span></span>

* <span data-ttu-id="4b951-337">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-337">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4b951-338">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-338">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="4b951-339">#4910</span><span class="sxs-lookup"><span data-stu-id="4b951-339">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="4b951-340">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-340">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="4b951-341">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="4b951-341">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4b951-342">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-342">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4b951-343">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-343">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4b951-344">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-344">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-345">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-345">Profile</span></span>

* <span data-ttu-id="4b951-346">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-346">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4b951-347">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-347">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b951-348">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b951-348">RDBMS</span></span>

* <span data-ttu-id="4b951-349">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-349">Added `georestore` command</span></span>
* <span data-ttu-id="4b951-350">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-350">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-351">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-351">Resource</span></span>

* <span data-ttu-id="4b951-352">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-352">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4b951-353">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-353">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-354">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-354">SQL</span></span>

* <span data-ttu-id="4b951-355">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-355">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-356">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-356">Storage</span></span>

* <span data-ttu-id="4b951-357">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-357">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-358">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-358">VM</span></span>

* <span data-ttu-id="4b951-359">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-359">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4b951-360">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-360">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4b951-362">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-362">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4b951-363">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-363">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="4b951-364">#5718</span><span class="sxs-lookup"><span data-stu-id="4b951-364">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="4b951-365">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-365">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4b951-366">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="4b951-366">March 27, 2018</span></span>

<span data-ttu-id="4b951-367">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4b951-367">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4b951-368">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-368">Core</span></span>

* <span data-ttu-id="4b951-369">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="4b951-369">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-370">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-370">ACS</span></span>

* <span data-ttu-id="4b951-371">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-371">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-372">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-372">Appservice</span></span>

* <span data-ttu-id="4b951-373">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-373">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4b951-374">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-374">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b951-375">Backup</span><span class="sxs-lookup"><span data-stu-id="4b951-375">Backup</span></span>

* <span data-ttu-id="4b951-376">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-376">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4b951-377">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-377">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4b951-378">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-378">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4b951-379">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-379">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b951-380">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-380">Container</span></span>

* <span data-ttu-id="4b951-381">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-381">Added `container exec` command.</span></span> <span data-ttu-id="4b951-382">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-382">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4b951-383">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-383">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-384">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-384">Extension</span></span>

* <span data-ttu-id="4b951-385">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-385">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4b951-386">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-386">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4b951-387">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-387">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-388">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-388">Interactive</span></span>

* <span data-ttu-id="4b951-389">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="4b951-389">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4b951-390">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-390">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4b951-391">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="4b951-391">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4b951-392">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-392">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4b951-393">랩</span><span class="sxs-lookup"><span data-stu-id="4b951-393">Lab</span></span>

* <span data-ttu-id="4b951-394">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-394">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-395">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-395">Monitor</span></span>

* <span data-ttu-id="4b951-396">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-396">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4b951-397">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="4b951-397">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4b951-398">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-398">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4b951-399">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-399">Network</span></span>

* <span data-ttu-id="4b951-400">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-400">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-401">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-401">Profile</span></span>

* <span data-ttu-id="4b951-402">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-402">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b951-403">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b951-403">RDBMS</span></span>

* <span data-ttu-id="4b951-404">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-404">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-405">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-405">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4b951-407">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-407">Role</span></span>

* <span data-ttu-id="4b951-408">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-408">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4b951-409">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-409">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4b951-410">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-410">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4b951-411">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-411">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4b951-412">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-412">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-413">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-413">Storage</span></span>

* <span data-ttu-id="4b951-414">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-414">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4b951-415">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="4b951-415">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-416">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-416">VM</span></span>

* <span data-ttu-id="4b951-417">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-417">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4b951-418">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-418">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4b951-419">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-419">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4b951-420">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-420">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4b951-421">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="4b951-421">March 13, 2018</span></span>

<span data-ttu-id="4b951-422">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4b951-422">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-423">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-423">ACR</span></span>

* <span data-ttu-id="4b951-424">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-424">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4b951-425">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-425">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4b951-426">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-426">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-427">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-427">ACS</span></span>

* <span data-ttu-id="4b951-428">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-428">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4b951-429">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-429">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4b951-430">Advisor</span><span class="sxs-lookup"><span data-stu-id="4b951-430">Advisor</span></span>

* <span data-ttu-id="4b951-431">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-431">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4b951-432">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-432">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4b951-433">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-433">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="4b951-434">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-434">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4b951-435">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-435">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-436">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-436">Appservice</span></span>

* <span data-ttu-id="4b951-437">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-437">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4b951-438">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-438">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4b951-439">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="4b951-439">Eventhubs</span></span>

* <span data-ttu-id="4b951-440">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-440">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-441">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-441">Extension</span></span>

* <span data-ttu-id="4b951-442">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-442">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-443">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-443">Interactive</span></span>

* <span data-ttu-id="4b951-444">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="4b951-444">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4b951-445">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="4b951-445">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4b951-446">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-446">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4b951-447">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-447">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-448">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-448">Monitor</span></span>

* <span data-ttu-id="4b951-449">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-449">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4b951-450">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-450">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4b951-451">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-451">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4b951-452">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-452">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b951-453">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-453">Network</span></span>

* <span data-ttu-id="4b951-454">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-454">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4b951-455">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="4b951-455">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4b951-456">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-456">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4b951-457">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-457">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-458">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-458">Profile</span></span>

* <span data-ttu-id="4b951-459">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-459">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4b951-460">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-460">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b951-461">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b951-461">RDBMS</span></span>

* <span data-ttu-id="4b951-462">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-462">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b951-463">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4b951-463">Service Bus</span></span>

* <span data-ttu-id="4b951-464">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-464">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-465">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-465">Storage</span></span>

* <span data-ttu-id="4b951-466">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-466">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4b951-467">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-467">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-468">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-468">VM</span></span>

* <span data-ttu-id="4b951-469">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-469">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4b951-470">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-470">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4b951-471">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-471">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4b951-472">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-472">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4b951-473">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="4b951-473">February 27, 2018</span></span>

<span data-ttu-id="4b951-474">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4b951-474">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4b951-475">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-475">Core</span></span>

* <span data-ttu-id="4b951-476">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-476">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4b951-477">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-477">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4b951-478">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-478">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-479">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-479">ACS</span></span>

* <span data-ttu-id="4b951-480">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-480">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4b951-481">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-481">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4b951-482">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-482">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4b951-483">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-483">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-484">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-484">Appservice</span></span>

* <span data-ttu-id="4b951-485">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4b951-485">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4b951-486">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-486">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b951-487">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b951-487">Cognitive Services</span></span>

* <span data-ttu-id="4b951-488">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="4b951-488">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4b951-489">Consumption</span><span class="sxs-lookup"><span data-stu-id="4b951-489">Consumption</span></span>

* <span data-ttu-id="4b951-490">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-490">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4b951-491">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="4b951-491">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4b951-492">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-492">Container</span></span>

* <span data-ttu-id="4b951-493">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-493">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4b951-494">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-494">Network</span></span>

* <span data-ttu-id="4b951-495">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-495">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-496">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-496">Resource</span></span>

* <span data-ttu-id="4b951-497">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-497">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4b951-498">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-498">Role</span></span>

* <span data-ttu-id="4b951-499">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-499">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-500">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-500">SQL</span></span>

* <span data-ttu-id="4b951-501">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-501">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-502">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-502">Storage</span></span>

* <span data-ttu-id="4b951-503">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="4b951-503">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-504">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-504">VM</span></span>

* <span data-ttu-id="4b951-505">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-505">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4b951-506">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="4b951-506">February 13, 2018</span></span>

<span data-ttu-id="4b951-507">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4b951-507">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4b951-508">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-508">Core</span></span>

* <span data-ttu-id="4b951-509">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-509">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-510">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-510">ACS</span></span>

* <span data-ttu-id="4b951-511">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-511">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4b951-512">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-512">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4b951-513">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-513">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4b951-514">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="4b951-514">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4b951-515">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-515">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4b951-516">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="4b951-516">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4b951-517">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-517">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4b951-518">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-518">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-519">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-519">Appservice</span></span>

* <span data-ttu-id="4b951-520">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-520">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4b951-521">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-521">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b951-522">CDN</span><span class="sxs-lookup"><span data-stu-id="4b951-522">CDN</span></span>

* <span data-ttu-id="4b951-523">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-523">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b951-524">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-524">Container</span></span>

* <span data-ttu-id="4b951-525">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-525">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4b951-526">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-526">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b951-527">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b951-527">CosmosDB</span></span>

* <span data-ttu-id="4b951-528">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-528">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-529">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-529">Extension</span></span>

* <span data-ttu-id="4b951-530">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-530">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4b951-531">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-531">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4b951-532">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="4b951-532">Feedback</span></span>

* <span data-ttu-id="4b951-533">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-533">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-534">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-534">Interactive</span></span>

* <span data-ttu-id="4b951-535">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-535">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4b951-536">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-536">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-537">IoT</span><span class="sxs-lookup"><span data-stu-id="4b951-537">IoT</span></span>

* <span data-ttu-id="4b951-538">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-538">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b951-539">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-539">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b951-540">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-540">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4b951-541">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-541">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-542">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-542">Monitor</span></span>

* <span data-ttu-id="4b951-543">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-543">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4b951-544">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-544">Network</span></span>

* <span data-ttu-id="4b951-545">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-545">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4b951-546">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-546">Profile</span></span>

* <span data-ttu-id="4b951-547">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-547">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-548">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-548">Resource</span></span>

* <span data-ttu-id="4b951-549">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-549">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4b951-550">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-550">Role</span></span>

* <span data-ttu-id="4b951-551">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-551">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-552">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-552">SQL</span></span>

* <span data-ttu-id="4b951-553">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-553">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4b951-554">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-554">Added `sql db rename`</span></span>
* <span data-ttu-id="4b951-555">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-555">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-556">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-556">Storage</span></span>

* <span data-ttu-id="4b951-557">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-557">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-558">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-558">VM</span></span>

* <span data-ttu-id="4b951-559">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-559">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4b951-560">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-560">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4b951-561">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="4b951-561">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4b951-562">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="4b951-562">January 31, 2018</span></span>

<span data-ttu-id="4b951-563">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4b951-563">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4b951-564">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-564">Core</span></span>

* <span data-ttu-id="4b951-565">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-565">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4b951-566">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-566">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4b951-567">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-567">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4b951-568">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="4b951-568">Use `--verbose` to see</span></span>
* <span data-ttu-id="4b951-569">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-569">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-570">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-570">ACS</span></span>

* <span data-ttu-id="4b951-571">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-571">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4b951-572">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="4b951-572">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-573">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-573">Appservice</span></span>

* <span data-ttu-id="4b951-574">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="4b951-574">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4b951-575">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-575">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4b951-576">CDN</span><span class="sxs-lookup"><span data-stu-id="4b951-576">CDN</span></span>

* <span data-ttu-id="4b951-577">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-577">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b951-578">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b951-578">CosmosDB</span></span>

* <span data-ttu-id="4b951-579">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-579">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-580">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-580">Interactive</span></span>

* <span data-ttu-id="4b951-581">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-581">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4b951-582">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-582">Network</span></span>

* <span data-ttu-id="4b951-583">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-583">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4b951-584">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-584">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4b951-585">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-585">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4b951-586">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-586">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4b951-587">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-587">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4b951-588">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="4b951-588">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4b951-589">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-589">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4b951-590">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-590">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4b951-591">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-591">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="4b951-592">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="4b951-592">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-593">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-593">Profile</span></span>

* <span data-ttu-id="4b951-594">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-594">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-595">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-595">Resource</span></span>

* <span data-ttu-id="4b951-596">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-596">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-597">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-597">Storage</span></span>

* <span data-ttu-id="4b951-598">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-598">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4b951-599">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-599">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4b951-600">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-600">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="4b951-601">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-601">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4b951-602">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-602">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-603">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-603">VM</span></span>

* <span data-ttu-id="4b951-604">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-604">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4b951-605">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-605">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4b951-606">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-606">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4b951-607">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-607">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4b951-608">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="4b951-608">January 17, 2018</span></span>

<span data-ttu-id="4b951-609">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4b951-609">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-610">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-610">ACR</span></span>

* <span data-ttu-id="4b951-611">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-611">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4b951-612">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-612">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-613">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-613">ACS</span></span>

* <span data-ttu-id="4b951-614">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-614">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4b951-615">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-615">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-616">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-616">Appservice</span></span>

* <span data-ttu-id="4b951-617">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-617">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4b951-618">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-618">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4b951-619">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-619">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4b951-620">Backup</span><span class="sxs-lookup"><span data-stu-id="4b951-620">Backup</span></span>

* <span data-ttu-id="4b951-621">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-621">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4b951-622">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-622">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4b951-623">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-623">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4b951-624">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-624">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4b951-625">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-625">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-626">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-626">Batch</span></span>

* <span data-ttu-id="4b951-627">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-627">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4b951-628">클라우드</span><span class="sxs-lookup"><span data-stu-id="4b951-628">Cloud</span></span>

* <span data-ttu-id="4b951-629">클라우드에서 `--profile`을 설정할 때 끝점을 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-629">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4b951-630">Consumption</span><span class="sxs-lookup"><span data-stu-id="4b951-630">Consumption</span></span>

* <span data-ttu-id="4b951-631">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-631">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b951-632">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b951-632">Event Grid</span></span>

* <span data-ttu-id="4b951-633">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="4b951-633">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b951-634">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="4b951-634">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b951-635">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-635">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4b951-636">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="4b951-636">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4b951-637">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-637">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4b951-638">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-638">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4b951-639">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-639">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4b951-640">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-640">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-641">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-641">Interactive</span></span>

* <span data-ttu-id="4b951-642">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-642">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4b951-643">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-643">Fixed errors on startup</span></span>
* <span data-ttu-id="4b951-644">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-644">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-645">IoT</span><span class="sxs-lookup"><span data-stu-id="4b951-645">IoT</span></span>

* <span data-ttu-id="4b951-646">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-646">Added support for device provisioning service</span></span>
* <span data-ttu-id="4b951-647">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-647">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4b951-648">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-648">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-649">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-649">Monitor</span></span>

* <span data-ttu-id="4b951-650">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-650">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4b951-651">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="4b951-651">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4b951-652">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-652">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4b951-653">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-653">Network</span></span>

* <span data-ttu-id="4b951-654">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-654">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4b951-655">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-655">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-656">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-656">Profile</span></span>

* <span data-ttu-id="4b951-657">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-657">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4b951-658">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-658">Role</span></span>

* <span data-ttu-id="4b951-659">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-659">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b951-660">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b951-660">Service Fabric</span></span>

* <span data-ttu-id="4b951-661">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-661">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4b951-662">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-662">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-663">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-663">VM</span></span>

* <span data-ttu-id="4b951-664">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-664">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4b951-665">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-665">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4b951-666">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-666">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4b951-667">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-667">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4b951-668">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-668">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4b951-669">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-669">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b951-670">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-670">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b951-671">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-671">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4b951-672">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="4b951-672">December 19, 2017</span></span>

<span data-ttu-id="4b951-673">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4b951-673">Version 2.0.23</span></span>

* <span data-ttu-id="4b951-674">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-674">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4b951-675">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-675">Container</span></span>

* <span data-ttu-id="4b951-676">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-676">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4b951-677">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-677">Network</span></span>

* <span data-ttu-id="4b951-678">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-678">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4b951-679">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-679">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-680">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-680">Storage</span></span>

* <span data-ttu-id="4b951-681">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-681">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-682">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-682">VM</span></span>

* <span data-ttu-id="4b951-683">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-683">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4b951-684">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="4b951-684">December 5, 2017</span></span>

<span data-ttu-id="4b951-685">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4b951-685">Version 2.0.22</span></span>

* <span data-ttu-id="4b951-686">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-686">Removed `az component` commands.</span></span> <span data-ttu-id="4b951-687">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="4b951-687">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4b951-688">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-688">Core</span></span>
* <span data-ttu-id="4b951-689">`AZURE_US_GOV_CLOUD` AAD 권한 끝점이 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-689">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4b951-690">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-690">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-691">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-691">ACS</span></span>

* <span data-ttu-id="4b951-692">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-692">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4b951-693">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-693">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4b951-694">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-694">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4b951-695">Advisor</span><span class="sxs-lookup"><span data-stu-id="4b951-695">Advisor</span></span>

* <span data-ttu-id="4b951-696">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-696">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-697">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-697">Appservice</span></span>

* <span data-ttu-id="4b951-698">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-698">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4b951-699">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-699">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4b951-700">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-700">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4b951-701">Consumption</span><span class="sxs-lookup"><span data-stu-id="4b951-701">Consumption</span></span>

* <span data-ttu-id="4b951-702">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-702">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4b951-703">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-703">Container</span></span>

* <span data-ttu-id="4b951-704">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-704">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-705">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-705">Monitor</span></span>

* <span data-ttu-id="4b951-706">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-706">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-707">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-707">Resource</span></span>

* <span data-ttu-id="4b951-708">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-708">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4b951-709">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-709">Role</span></span>

* <span data-ttu-id="4b951-710">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-710">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4b951-711">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-711">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4b951-712">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="4b951-712">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-713">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-713">SQL</span></span>

* <span data-ttu-id="4b951-714">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-714">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4b951-715">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-715">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-716">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-716">VM</span></span>

* <span data-ttu-id="4b951-717">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-717">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4b951-718">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="4b951-718">November 14, 2017</span></span>

<span data-ttu-id="4b951-719">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4b951-719">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-720">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-720">ACR</span></span>

* <span data-ttu-id="4b951-721">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-721">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4b951-722">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-722">ACS</span></span>

* <span data-ttu-id="4b951-723">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-723">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4b951-724">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="4b951-724">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4b951-725">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-725">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4b951-726">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-726">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4b951-727">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-727">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-728">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-728">Appservice</span></span>

* <span data-ttu-id="4b951-729">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-729">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4b951-730">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-730">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4b951-731">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-731">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4b951-732">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-732">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4b951-733">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-733">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4b951-734">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="4b951-734">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-735">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-735">Batch</span></span>

* <span data-ttu-id="4b951-736">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-736">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4b951-737">Batchai</span><span class="sxs-lookup"><span data-stu-id="4b951-737">Batchai</span></span>

* <span data-ttu-id="4b951-738">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-738">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4b951-739">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-739">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4b951-740">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-740">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4b951-741">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-741">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4b951-742">클라우드</span><span class="sxs-lookup"><span data-stu-id="4b951-742">Cloud</span></span>

* <span data-ttu-id="4b951-743">필요한 끝점이 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-743">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4b951-744">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-744">Container</span></span>

* <span data-ttu-id="4b951-745">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-745">Added support to open multiple ports</span></span>
* <span data-ttu-id="4b951-746">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-746">Added container group restart policy</span></span>
* <span data-ttu-id="4b951-747">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-747">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4b951-748">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="4b951-748">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b951-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b951-749">Data Lake Analytics</span></span>

* <span data-ttu-id="4b951-750">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-750">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b951-751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b951-751">Data Lake Store</span></span>

* <span data-ttu-id="4b951-752">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-752">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-753">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-753">Extension</span></span>

* <span data-ttu-id="4b951-754">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-754">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4b951-755">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-755">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-756">IoT</span><span class="sxs-lookup"><span data-stu-id="4b951-756">IoT</span></span>

* <span data-ttu-id="4b951-757">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-757">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-758">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-758">Monitor</span></span>

* <span data-ttu-id="4b951-759">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-759">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b951-760">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-760">Network</span></span>

* <span data-ttu-id="4b951-761">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-761">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4b951-762">`traffic-manager profile update`로 끝점을 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-762">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4b951-763">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-763">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4b951-764">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-764">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4b951-765">예약</span><span class="sxs-lookup"><span data-stu-id="4b951-765">Reservations</span></span>

* <span data-ttu-id="4b951-766">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-766">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-767">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-767">Resource</span></span>

* <span data-ttu-id="4b951-768">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-768">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-769">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-769">SQL</span></span>

* <span data-ttu-id="4b951-770">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-770">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-771">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-771">Storage</span></span>

* <span data-ttu-id="4b951-772">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-772">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4b951-773">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-773">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4b951-774">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-774">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4b951-775">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="4b951-775">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4b951-776">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-776">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4b951-777">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-777">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4b951-778">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-778">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-779">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-779">VM</span></span>

* <span data-ttu-id="4b951-780">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-780">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4b951-781">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-781">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4b951-782">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-782">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4b951-783">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-783">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4b951-784">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-784">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4b951-785">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="4b951-785">October 24, 2017</span></span>

<span data-ttu-id="4b951-786">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4b951-786">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4b951-787">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-787">Core</span></span>

* <span data-ttu-id="4b951-788">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="4b951-788">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-789">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-789">ACR</span></span>

* <span data-ttu-id="4b951-790">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="4b951-790">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4b951-791">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-791">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4b951-792">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="4b951-792">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-793">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-793">ACS</span></span>

* <span data-ttu-id="4b951-794">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-794">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4b951-795">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-795">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-796">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-796">Appservice</span></span>

* <span data-ttu-id="4b951-797">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-797">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4b951-798">구성 요소</span><span class="sxs-lookup"><span data-stu-id="4b951-798">Component</span></span>

* <span data-ttu-id="4b951-799">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-799">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-800">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-800">Monitor</span></span>

* <span data-ttu-id="4b951-801">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-801">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-802">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-802">Resource</span></span>

* <span data-ttu-id="4b951-803">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-803">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4b951-804">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-804">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-805">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-805">VM</span></span>

* <span data-ttu-id="4b951-806">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-806">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4b951-807">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="4b951-807">October 9, 2017</span></span>

<span data-ttu-id="4b951-808">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4b951-808">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4b951-809">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-809">Core</span></span>

* <span data-ttu-id="4b951-810">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-810">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-811">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-811">Appservice</span></span>

* <span data-ttu-id="4b951-812">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-812">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-813">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-813">Batch</span></span>

* <span data-ttu-id="4b951-814">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-814">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4b951-815">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-815">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4b951-816">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-816">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4b951-817">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-817">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4b951-818">Batchai</span><span class="sxs-lookup"><span data-stu-id="4b951-818">Batchai</span></span>

* <span data-ttu-id="4b951-819">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-819">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-820">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b951-820">Keyvault</span></span>

* <span data-ttu-id="4b951-821">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-821">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4b951-822">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4b951-822">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4b951-823">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-823">Network</span></span>

* <span data-ttu-id="4b951-824">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-824">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4b951-825">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-825">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-826">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-826">Resource</span></span>

* <span data-ttu-id="4b951-827">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-827">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4b951-828">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-828">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4b951-829">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-829">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4b951-830">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-830">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-831">Sql</span><span class="sxs-lookup"><span data-stu-id="4b951-831">Sql</span></span>

* <span data-ttu-id="4b951-832">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-832">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4b951-833">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-833">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4b951-834">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-834">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-835">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-835">Storage</span></span>

* <span data-ttu-id="4b951-836">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-836">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-837">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-837">Vm</span></span>

* <span data-ttu-id="4b951-838">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-838">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4b951-839">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-839">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4b951-840">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-840">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4b951-841">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-841">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4b951-842">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-842">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4b951-843">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="4b951-843">September 22, 2017</span></span>

<span data-ttu-id="4b951-844">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4b951-844">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-845">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-845">Resource</span></span>

* <span data-ttu-id="4b951-846">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-846">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4b951-847">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-847">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4b951-848">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-848">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4b951-849">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-849">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4b951-850">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-850">Network</span></span>

* <span data-ttu-id="4b951-851">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-851">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4b951-852">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-852">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4b951-853">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-853">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4b951-854">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-854">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4b951-855">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-855">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b951-856">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-856">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4b951-857">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-857">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-858">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-858">Storage</span></span>

* <span data-ttu-id="4b951-859">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-859">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4b951-860">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b951-860">Eventgrid</span></span>

* <span data-ttu-id="4b951-861">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="4b951-861">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-862">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-862">SQL</span></span>

* <span data-ttu-id="4b951-863">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-863">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4b951-864">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="4b951-864">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4b951-865">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-865">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-866">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b951-866">Keyvault</span></span>

* <span data-ttu-id="4b951-867">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-867">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-868">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-868">VM</span></span>

* <span data-ttu-id="4b951-869">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-869">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4b951-870">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4b951-870">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4b951-871">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-871">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4b951-872">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-872">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4b951-873">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-873">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4b951-874">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-874">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-875">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-875">ACS</span></span>

* <span data-ttu-id="4b951-876">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-876">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-877">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-877">Appservice</span></span>

* <span data-ttu-id="4b951-878">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-878">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b951-879">Backup</span><span class="sxs-lookup"><span data-stu-id="4b951-879">Backup</span></span>

* <span data-ttu-id="4b951-880">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-880">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4b951-881">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="4b951-881">September 11, 2017</span></span>

<span data-ttu-id="4b951-882">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4b951-882">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4b951-883">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-883">Core</span></span>

* <span data-ttu-id="4b951-884">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-884">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4b951-885">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-885">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-886">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-886">Acs</span></span>

* <span data-ttu-id="4b951-887">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-887">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4b951-888">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="4b951-888">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-889">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-889">Appservice</span></span>

* <span data-ttu-id="4b951-890">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-890">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4b951-891">CDN</span><span class="sxs-lookup"><span data-stu-id="4b951-891">CDN</span></span>

* <span data-ttu-id="4b951-892">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-892">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4b951-893">내선 번호</span><span class="sxs-lookup"><span data-stu-id="4b951-893">Extension</span></span>

* <span data-ttu-id="4b951-894">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-894">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-895">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b951-895">Keyvault</span></span>

* <span data-ttu-id="4b951-896">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-896">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4b951-897">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-897">Network</span></span>

* <span data-ttu-id="4b951-898">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-898">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b951-899">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-899">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4b951-900">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-900">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4b951-901">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-901">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b951-902">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-902">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-903">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-903">Resource</span></span>

* <span data-ttu-id="4b951-904">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-904">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4b951-905">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-905">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4b951-906">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-906">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4b951-907">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="4b951-907">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-908">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-908">SQL</span></span>

* <span data-ttu-id="4b951-909">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-909">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-910">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-910">VM</span></span>

* <span data-ttu-id="4b951-911">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-911">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4b951-912">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="4b951-912">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4b951-913">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-913">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4b951-914">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-914">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4b951-915">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-915">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4b951-916">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="4b951-916">August 31, 2017</span></span>

<span data-ttu-id="4b951-917">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4b951-917">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-918">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b951-918">Keyvault</span></span>

* <span data-ttu-id="4b951-919">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-919">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4b951-920">Sf</span><span class="sxs-lookup"><span data-stu-id="4b951-920">Sf</span></span>

* <span data-ttu-id="4b951-921">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-921">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-922">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-922">Storage</span></span>

* <span data-ttu-id="4b951-923">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-923">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4b951-924">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="4b951-924">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4b951-925">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="4b951-925">August 28, 2017</span></span>

<span data-ttu-id="4b951-926">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4b951-926">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4b951-927">CLI</span><span class="sxs-lookup"><span data-stu-id="4b951-927">CLI</span></span>

* <span data-ttu-id="4b951-928">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-928">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-929">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-929">ACS</span></span>

* <span data-ttu-id="4b951-930">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-930">Corrected preview regions</span></span>
* <span data-ttu-id="4b951-931">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-931">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4b951-932">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="4b951-932">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-933">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-933">Appservice</span></span>

* <span data-ttu-id="4b951-934">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-934">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4b951-935">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-935">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4b951-936">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-936">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4b951-937">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-937">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4b951-938">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-938">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-939">IoT</span><span class="sxs-lookup"><span data-stu-id="4b951-939">IoT</span></span>

* <span data-ttu-id="4b951-940">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-940">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4b951-941">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-941">Network</span></span>

* <span data-ttu-id="4b951-942">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-942">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b951-943">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-943">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4b951-944">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-944">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b951-945">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-945">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b951-946">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-946">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-947">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-947">Profile</span></span>

* <span data-ttu-id="4b951-948">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-948">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b951-949">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b951-949">Service Fabric</span></span>

* <span data-ttu-id="4b951-950">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-950">Preview release</span></span>
* <span data-ttu-id="4b951-951">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="4b951-951">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4b951-952">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-952">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4b951-953">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-953">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-954">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-954">Storage</span></span>

* <span data-ttu-id="4b951-955">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-955">Enabled setting blob tier</span></span>
* <span data-ttu-id="4b951-956">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-956">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4b951-957">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-957">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4b951-958">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-958">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4b951-959">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-959">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4b951-960">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-960">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-961">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-961">VM</span></span>

* <span data-ttu-id="4b951-962">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-962">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4b951-963">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-963">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4b951-964">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-964">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b951-965">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-965">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4b951-966">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-966">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4b951-967">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-967">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4b951-968">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="4b951-968">August 15, 2017</span></span>

<span data-ttu-id="4b951-969">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4b951-969">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-970">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-970">ACS</span></span>

* <span data-ttu-id="4b951-971">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-971">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-972">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-972">Appservice</span></span>

* <span data-ttu-id="4b951-973">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-973">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b951-974">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b951-974">Event Grid</span></span>

* <span data-ttu-id="4b951-975">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-975">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4b951-976">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="4b951-976">August 11, 2017</span></span>

<span data-ttu-id="4b951-977">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4b951-977">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-978">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-978">ACS</span></span>

* <span data-ttu-id="4b951-979">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-979">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-980">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-980">Batch</span></span>

* <span data-ttu-id="4b951-981">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-981">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4b951-982">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-982">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4b951-983">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-983">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4b951-984">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-984">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4b951-985">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-985">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4b951-986">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-986">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4b951-987">구성 요소</span><span class="sxs-lookup"><span data-stu-id="4b951-987">Component</span></span>

* <span data-ttu-id="4b951-988">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-988">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4b951-989">컨테이너</span><span class="sxs-lookup"><span data-stu-id="4b951-989">Container</span></span>

* <span data-ttu-id="4b951-990">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-990">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4b951-991">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b951-991">Data Lake Store</span></span>

* <span data-ttu-id="4b951-992">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-992">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b951-993">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b951-993">Event Grid</span></span>

* <span data-ttu-id="4b951-994">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-994">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4b951-995">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-995">Network</span></span>

* <span data-ttu-id="4b951-996">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-996">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4b951-997">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-997">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4b951-998">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-998">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4b951-999">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-999">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-1000">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-1000">Profile</span></span>

* <span data-ttu-id="4b951-1001">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1001">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-1002">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-1002">Storage</span></span>

* <span data-ttu-id="4b951-1003">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1003">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-1004">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-1004">VM</span></span>

* <span data-ttu-id="4b951-1005">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1005">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4b951-1006">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1006">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4b951-1007">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1007">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4b951-1008">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1008">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4b951-1009">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1009">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4b951-1010">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="4b951-1010">July 28, 2017</span></span>

<span data-ttu-id="4b951-1011">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4b951-1011">Version 2.0.12</span></span>

* <span data-ttu-id="4b951-1012">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1012">Added container commands</span></span>
* <span data-ttu-id="4b951-1013">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1013">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4b951-1014">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-1014">Core</span></span>

* <span data-ttu-id="4b951-1015">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1015">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4b951-1016">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1016">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4b951-1017">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="4b951-1017">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4b951-1018">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="4b951-1018">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4b951-1019">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="4b951-1019">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4b951-1020">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="4b951-1020">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4b951-1021">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="4b951-1021">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b951-1022">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="4b951-1022">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4b951-1023">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="4b951-1023">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4b951-1024">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="4b951-1024">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4b951-1025">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="4b951-1025">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4b951-1026">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="4b951-1026">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4b951-1027">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-1027">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4b951-1028">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-1028">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4b951-1029">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1029">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4b951-1030">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="4b951-1030">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4b951-1031">ACR</span><span class="sxs-lookup"><span data-stu-id="4b951-1031">ACR</span></span>

* <span data-ttu-id="4b951-1032">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1032">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4b951-1033">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1033">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4b951-1034">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1034">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4b951-1035">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1035">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4b951-1036">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1036">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4b951-1037">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1037">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-1038">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-1038">ACS</span></span>

* <span data-ttu-id="4b951-1039">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1039">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-1040">App Service</span><span class="sxs-lookup"><span data-stu-id="4b951-1040">Appservice</span></span>

* <span data-ttu-id="4b951-1041">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1041">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4b951-1042">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1042">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4b951-1043">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1043">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4b951-1044">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="4b951-1044">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4b951-1045">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="4b951-1045">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4b951-1046">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="4b951-1046">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4b951-1047">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="4b951-1047">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4b951-1048">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="4b951-1048">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4b951-1049">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1049">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4b951-1050">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1050">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4b951-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="4b951-1051">Batch</span></span>

* <span data-ttu-id="4b951-1052">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1052">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4b951-1053">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1053">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4b951-1054">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1054">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b951-1055">CDN</span><span class="sxs-lookup"><span data-stu-id="4b951-1055">CDN</span></span>

* <span data-ttu-id="4b951-1056">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1056">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4b951-1057">클라우드</span><span class="sxs-lookup"><span data-stu-id="4b951-1057">Cloud</span></span>

* <span data-ttu-id="4b951-1058">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1058">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4b951-1059">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-1059">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4b951-1060">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1060">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4b951-1061">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1061">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4b951-1062">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1062">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b951-1063">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b951-1063">CosmosDB</span></span>

* <span data-ttu-id="4b951-1064">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1064">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4b951-1065">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1065">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b951-1066">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b951-1066">Data Lake Analytics</span></span>

* <span data-ttu-id="4b951-1067">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1067">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4b951-1068">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1068">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4b951-1069">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1069">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b951-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b951-1070">Data Lake Store</span></span>

* <span data-ttu-id="4b951-1071">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1071">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4b951-1072">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1072">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4b951-1073">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1073">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4b951-1074">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="4b951-1074">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4b951-1075">대화형</span><span class="sxs-lookup"><span data-stu-id="4b951-1075">Interactive</span></span>

* <span data-ttu-id="4b951-1076">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1076">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4b951-1077">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1077">Increased test coverage</span></span>
* <span data-ttu-id="4b951-1078">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1078">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4b951-1079">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="4b951-1079">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4b951-1080">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="4b951-1080">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4b951-1081">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="4b951-1081">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4b951-1082">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="4b951-1082">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b951-1083">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1083">Added `--progress` flag</span></span>
* <span data-ttu-id="4b951-1084">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1084">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4b951-1085">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="4b951-1085">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4b951-1086">IoT</span><span class="sxs-lookup"><span data-stu-id="4b951-1086">IoT</span></span>

* <span data-ttu-id="4b951-1087">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1087">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4b951-1088">(#3934)</span><span class="sxs-lookup"><span data-stu-id="4b951-1088">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b951-1089">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="4b951-1089">Key vault</span></span>

* <span data-ttu-id="4b951-1090">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="4b951-1090">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4b951-1091">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b951-1091">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4b951-1092">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b951-1092">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b951-1093">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b951-1093">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b951-1094">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b951-1094">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4b951-1095">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="4b951-1095">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4b951-1096">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1096">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4b951-1097">(#3307)</span><span class="sxs-lookup"><span data-stu-id="4b951-1097">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4b951-1098">랩</span><span class="sxs-lookup"><span data-stu-id="4b951-1098">Lab</span></span>

* <span data-ttu-id="4b951-1099">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1099">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4b951-1100">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1100">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-1101">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-1101">Monitor</span></span>

* <span data-ttu-id="4b951-1102">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="4b951-1102">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4b951-1103">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1103">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4b951-1104">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1104">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4b951-1105">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1105">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4b951-1106">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1106">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4b951-1107">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="4b951-1107">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4b951-1108">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1108">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4b951-1109">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1109">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4b951-1110">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1110">`location` no longer required</span></span>
  * <span data-ttu-id="4b951-1111">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1111">Add name and ID support for target</span></span>
  * <span data-ttu-id="4b951-1112">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1112">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4b951-1113">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1113">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4b951-1114">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1114">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4b951-1115">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1115">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4b951-1116">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1116">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4b951-1117">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1117">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4b951-1118">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-1118">Network</span></span>

* <span data-ttu-id="4b951-1119">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1119">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4b951-1120">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1120">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4b951-1121">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1121">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4b951-1122">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1122">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4b951-1123">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1123">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4b951-1124">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1124">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4b951-1125">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4b951-1125">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4b951-1126">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4b951-1126">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4b951-1127">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4b951-1127">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4b951-1128">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b951-1128">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4b951-1129">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b951-1129">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4b951-1130">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="4b951-1130">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4b951-1131">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4b951-1131">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4b951-1132">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b951-1132">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4b951-1133">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1133">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4b951-1134">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1134">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4b951-1135">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1135">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4b951-1136">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1136">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4b951-1137">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1137">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4b951-1138">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1138">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4b951-1139">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1139">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4b951-1140">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1140">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4b951-1141">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1141">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4b951-1142">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1142">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4b951-1143">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1143">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4b951-1144">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1144">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4b951-1145">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1145">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-1146">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-1146">Profile</span></span>

* <span data-ttu-id="4b951-1147">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1147">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4b951-1148">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1148">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4b951-1149">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1149">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4b951-1150">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1150">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4b951-1151">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1151">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b951-1152">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b951-1152">RDBMS</span></span>

* <span data-ttu-id="4b951-1153">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="4b951-1153">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4b951-1154">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="4b951-1154">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4b951-1155">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="4b951-1155">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4b951-1156">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="4b951-1156">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-1157">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-1157">Resource</span></span>

* <span data-ttu-id="4b951-1158">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1158">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4b951-1159">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1159">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4b951-1160">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1160">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4b951-1161">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1161">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4b951-1162">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="4b951-1162">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4b951-1163">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1163">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4b951-1164">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="4b951-1164">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4b951-1165">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1165">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4b951-1166">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-1166">Role</span></span>

* <span data-ttu-id="4b951-1167">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1167">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4b951-1168">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="4b951-1168">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4b951-1169">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1169">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4b951-1170">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1170">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4b951-1171">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1171">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b951-1172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b951-1172">Service Fabric</span></span>
* <span data-ttu-id="4b951-1173">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="4b951-1173">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4b951-1174">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="4b951-1174">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4b951-1175">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="4b951-1175">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-1176">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-1176">SQL</span></span>

* <span data-ttu-id="4b951-1177">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1177">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4b951-1178">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1178">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4b951-1179">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1179">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-1180">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-1180">Storage</span></span>

* <span data-ttu-id="4b951-1181">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="4b951-1181">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4b951-1182">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="4b951-1182">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4b951-1183">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="4b951-1183">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4b951-1184">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1184">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4b951-1185">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="4b951-1185">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4b951-1186">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="4b951-1186">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-1187">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-1187">VM</span></span>

* <span data-ttu-id="4b951-1188">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1188">Support configuring nsg</span></span>
* <span data-ttu-id="4b951-1189">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1189">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4b951-1190">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1190">Support managed service identities</span></span>
* <span data-ttu-id="4b951-1191">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1191">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4b951-1192">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1192">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4b951-1193">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="4b951-1193">May 10, 2017</span></span>

<span data-ttu-id="4b951-1194">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4b951-1194">Version 2.0.6</span></span>

* <span data-ttu-id="4b951-1195">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="4b951-1195">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4b951-1196">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1196">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4b951-1197">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="4b951-1197">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4b951-1198">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="4b951-1198">Include Cognitive Services module</span></span>
* <span data-ttu-id="4b951-1199">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="4b951-1199">Include Service Fabric module</span></span>
* <span data-ttu-id="4b951-1200">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="4b951-1200">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4b951-1201">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1201">Add support for CDN commands</span></span>
* <span data-ttu-id="4b951-1202">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-1202">Remove Container module</span></span>
* <span data-ttu-id="4b951-1203">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="4b951-1203">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4b951-1204">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b951-1204">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4b951-1205">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-1205">Core</span></span>

* <span data-ttu-id="4b951-1206">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="4b951-1206">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4b951-1207">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4b951-1207">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4b951-1208">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4b951-1208">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4b951-1209">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4b951-1209">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4b951-1210">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4b951-1210">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4b951-1211">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4b951-1211">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4b951-1212">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4b951-1212">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4b951-1213">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4b951-1213">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4b951-1214">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4b951-1214">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4b951-1215">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="4b951-1215">core: Improved performance</span></span>
* <span data-ttu-id="4b951-1216">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1216">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4b951-1217">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="4b951-1217">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-1218">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-1218">ACS</span></span>

* <span data-ttu-id="4b951-1219">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1219">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4b951-1220">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="4b951-1220">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4b951-1221">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="4b951-1221">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4b951-1222">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4b951-1222">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-1223">AppService</span><span class="sxs-lookup"><span data-stu-id="4b951-1223">AppService</span></span>

* <span data-ttu-id="4b951-1224">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="4b951-1224">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4b951-1225">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1225">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4b951-1226">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="4b951-1226">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4b951-1227">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="4b951-1227">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4b951-1228">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="4b951-1228">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4b951-1229">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4b951-1229">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4b951-1230">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1230">support slot swap with preview</span></span>
* <span data-ttu-id="4b951-1231">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4b951-1231">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4b951-1232">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4b951-1232">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b951-1233">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b951-1233">CosmosDB</span></span>

* <span data-ttu-id="4b951-1234">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="4b951-1234">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4b951-1235">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1235">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4b951-1236">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1236">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4b951-1237">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1237">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b951-1238">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b951-1238">Data Lake Analytics</span></span>

* <span data-ttu-id="4b951-1239">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1239">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4b951-1240">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1240">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4b951-1241">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="4b951-1241">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4b951-1242">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="4b951-1242">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4b951-1243">테이블</span><span class="sxs-lookup"><span data-stu-id="4b951-1243">Table</span></span>
  * <span data-ttu-id="4b951-1244">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="4b951-1244">Table valued function</span></span>
  * <span data-ttu-id="4b951-1245">보기</span><span class="sxs-lookup"><span data-stu-id="4b951-1245">View</span></span>
  * <span data-ttu-id="4b951-1246">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="4b951-1246">Table Statistics.</span></span> <span data-ttu-id="4b951-1247">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="4b951-1247">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b951-1248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b951-1248">Data Lake Store</span></span>

* <span data-ttu-id="4b951-1249">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="4b951-1249">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4b951-1250">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b951-1250">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4b951-1251">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="4b951-1251">missed help for access show.</span></span> <span data-ttu-id="4b951-1252">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1252">adding it.</span></span> <span data-ttu-id="4b951-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4b951-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4b951-1254">찾기</span><span class="sxs-lookup"><span data-stu-id="4b951-1254">Find</span></span>

* <span data-ttu-id="4b951-1255">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="4b951-1255">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b951-1256">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b951-1256">KeyVault</span></span>

* <span data-ttu-id="4b951-1257">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1257">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4b951-1258">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1258">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4b951-1259">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1259">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4b951-1260">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1260">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4b951-1261">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4b951-1261">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4b951-1262">랩</span><span class="sxs-lookup"><span data-stu-id="4b951-1262">Lab</span></span>

* <span data-ttu-id="4b951-1263">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1263">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4b951-1264">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1264">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4b951-1265">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="4b951-1265">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4b951-1266">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="4b951-1266">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4b951-1267">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1267">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4b951-1268">모니터</span><span class="sxs-lookup"><span data-stu-id="4b951-1268">Monitor</span></span>

* <span data-ttu-id="4b951-1269">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4b951-1269">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4b951-1270">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4b951-1270">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4b951-1271">네트워크</span><span class="sxs-lookup"><span data-stu-id="4b951-1271">Network</span></span>

* <span data-ttu-id="4b951-1272">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1272">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4b951-1273">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1273">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4b951-1274">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1274">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4b951-1275">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1275">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4b951-1276">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1276">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4b951-1277">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1277">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4b951-1278">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1278">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4b951-1279">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1279">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4b951-1280">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1280">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4b951-1281">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1281">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4b951-1282">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="4b951-1282">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4b951-1283">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1283">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4b951-1284">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1284">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4b951-1285">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1285">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4b951-1286">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="4b951-1286">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4b951-1287">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1287">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b951-1288">프로필</span><span class="sxs-lookup"><span data-stu-id="4b951-1288">Profile</span></span>

* <span data-ttu-id="4b951-1289">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4b951-1289">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4b951-1290">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4b951-1290">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4b951-1291">Redis</span><span class="sxs-lookup"><span data-stu-id="4b951-1291">Redis</span></span>

* <span data-ttu-id="4b951-1292">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1292">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4b951-1293">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="4b951-1293">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4b951-1294">리소스</span><span class="sxs-lookup"><span data-stu-id="4b951-1294">Resource</span></span>

* <span data-ttu-id="4b951-1295">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4b951-1295">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4b951-1296">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4b951-1296">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4b951-1297">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4b951-1297">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4b951-1298">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1298">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4b951-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4b951-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4b951-1300">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1300">Add docs for az lock update.</span></span> <span data-ttu-id="4b951-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4b951-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4b951-1302">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1302">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4b951-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4b951-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4b951-1304">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1304">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4b951-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4b951-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4b951-1306">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4b951-1306">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4b951-1307">역할</span><span class="sxs-lookup"><span data-stu-id="4b951-1307">Role</span></span>

* <span data-ttu-id="4b951-1308">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4b951-1308">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4b951-1309">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4b951-1309">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4b951-1310">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4b951-1310">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4b951-1311">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="4b951-1311">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4b951-1312">SQL</span><span class="sxs-lookup"><span data-stu-id="4b951-1312">SQL</span></span>

* <span data-ttu-id="4b951-1313">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="4b951-1313">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4b951-1314">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4b951-1314">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4b951-1315">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-1315">Storage</span></span>

* <span data-ttu-id="4b951-1316">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="4b951-1316">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4b951-1317">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1317">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4b951-1318">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1318">Add support for large block blob upload</span></span>
* <span data-ttu-id="4b951-1319">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="4b951-1319">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-1320">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-1320">VM</span></span>

* <span data-ttu-id="4b951-1321">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="4b951-1321">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4b951-1322">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="4b951-1322">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4b951-1323">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4b951-1323">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4b951-1324">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4b951-1324">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4b951-1325">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1325">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4b951-1326">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="4b951-1326">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4b951-1327">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4b951-1327">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4b951-1328">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="4b951-1328">April 3, 2017</span></span>

<span data-ttu-id="4b951-1329">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4b951-1329">Version 2.0.2</span></span>

<span data-ttu-id="4b951-1330">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1330">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4b951-1331">코어</span><span class="sxs-lookup"><span data-stu-id="4b951-1331">Core</span></span>

* <span data-ttu-id="4b951-1332">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="4b951-1332">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4b951-1333">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4b951-1333">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4b951-1334">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4b951-1334">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4b951-1335">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b951-1335">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b951-1336">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4b951-1336">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4b951-1337">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="4b951-1337">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4b951-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4b951-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4b951-1339">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1339">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4b951-1340">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="4b951-1340">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4b951-1341">ACS</span><span class="sxs-lookup"><span data-stu-id="4b951-1341">ACS</span></span>

* <span data-ttu-id="4b951-1342">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4b951-1342">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4b951-1343">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="4b951-1343">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4b951-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4b951-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4b951-1345">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="4b951-1345">Add support for windows clusters.</span></span> <span data-ttu-id="4b951-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4b951-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4b951-1347">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="4b951-1347">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4b951-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4b951-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b951-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="4b951-1349">AppService</span></span>

* <span data-ttu-id="4b951-1350">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4b951-1350">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4b951-1351">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4b951-1351">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4b951-1352">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4b951-1352">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4b951-1353">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4b951-1353">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4b951-1354">DataLake</span><span class="sxs-lookup"><span data-stu-id="4b951-1354">DataLake</span></span>

* <span data-ttu-id="4b951-1355">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-1355">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4b951-1356">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="4b951-1356">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4b951-1357">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="4b951-1357">DocuemntDB</span></span>

* <span data-ttu-id="4b951-1358">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4b951-1358">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4b951-1359">VM</span><span class="sxs-lookup"><span data-stu-id="4b951-1359">VM</span></span>

* <span data-ttu-id="4b951-1360">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4b951-1360">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4b951-1361">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4b951-1361">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4b951-1362">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4b951-1362">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4b951-1363">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b951-1363">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b951-1364">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4b951-1364">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4b951-1365">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="4b951-1365">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4b951-1366">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4b951-1366">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4b951-1367">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="4b951-1367">February 27, 2017</span></span>

<span data-ttu-id="4b951-1368">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4b951-1368">Version 2.0.0</span></span>

<span data-ttu-id="4b951-1369">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1369">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4b951-1370">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="4b951-1370">Container Service (acs)</span></span>
- <span data-ttu-id="4b951-1371">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="4b951-1371">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4b951-1372">네트워킹</span><span class="sxs-lookup"><span data-stu-id="4b951-1372">Networking</span></span>
- <span data-ttu-id="4b951-1373">Storage</span><span class="sxs-lookup"><span data-stu-id="4b951-1373">Storage</span></span>

<span data-ttu-id="4b951-1374">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1374">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4b951-1375">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1375">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4b951-1376">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1376">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4b951-1377">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1377">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4b951-1378">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4b951-1378">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4b951-1379">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4b951-1379">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4b951-1380">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="4b951-1380">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4b951-1381">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="4b951-1381">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4b951-1382">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="4b951-1382">Provide feedback from the command line with the `az feedback` command</span></span>


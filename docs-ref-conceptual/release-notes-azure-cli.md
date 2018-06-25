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
ms.openlocfilehash: 64db2b58ca883518757d8e189bf7263ed818b283
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262661"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="5bdad-103">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="5bdad-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5bdad-104">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="5bdad-104">June 19, 2018</span></span>

<span data-ttu-id="5bdad-105">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5bdad-105">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-106">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-106">Core</span></span>

* <span data-ttu-id="5bdad-107">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-107">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-108">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-108">ACR</span></span>

* <span data-ttu-id="5bdad-109">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-109">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5bdad-110">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-110">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-111">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-111">ACS</span></span>

* <span data-ttu-id="5bdad-112">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="5bdad-112">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5bdad-113">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-113">Added `--update` support</span></span>
* <span data-ttu-id="5bdad-114">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-114">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5bdad-115">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="5bdad-115">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5bdad-116">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-116">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5bdad-117">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-117">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5bdad-118">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-118">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5bdad-119">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-119">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span> 

### <a name="appservice"></a><span data-ttu-id="5bdad-120">AppService</span><span class="sxs-lookup"><span data-stu-id="5bdad-120">AppService</span></span>

* <span data-ttu-id="5bdad-121">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-121">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5bdad-122">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-122">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-123">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-123">Batch</span></span>

* <span data-ttu-id="5bdad-124">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-124">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bdad-125">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5bdad-125">Batch AI</span></span>

* <span data-ttu-id="5bdad-126">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="5bdad-126">Added support for workspaces.</span></span> <span data-ttu-id="5bdad-127">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-127">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5bdad-128">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="5bdad-128">Added support for experiments.</span></span> <span data-ttu-id="5bdad-129">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-129">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5bdad-130">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-130">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5bdad-131">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="5bdad-131">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5bdad-132">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-132">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5bdad-133">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-133">Added support for `--ids` to `batchai` commands</span></span> 
* <span data-ttu-id="5bdad-134">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="5bdad-134">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5bdad-135">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="5bdad-135">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5bdad-136">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="5bdad-136">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5bdad-137">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="5bdad-137">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5bdad-138">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="5bdad-138">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5bdad-139">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="5bdad-139">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5bdad-140">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="5bdad-140">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5bdad-141">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-141">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5bdad-142">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-142">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5bdad-143">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="5bdad-143">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="5bdad-144">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="5bdad-144">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="5bdad-145">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="5bdad-145">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="5bdad-146">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="5bdad-146">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="5bdad-147">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="5bdad-147">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5bdad-148">지도</span><span class="sxs-lookup"><span data-stu-id="5bdad-148">Maps</span></span>

* <span data-ttu-id="5bdad-149">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-149">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-150">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-150">Network</span></span>

* <span data-ttu-id="5bdad-151">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-151">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5bdad-152">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-152">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5bdad-153">#6502</span><span class="sxs-lookup"><span data-stu-id="5bdad-153">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5bdad-154">예약</span><span class="sxs-lookup"><span data-stu-id="5bdad-154">Reservations</span></span>

* <span data-ttu-id="5bdad-155">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-155">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5bdad-156">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-156">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5bdad-157">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-157">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5bdad-158">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-158">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5bdad-159">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-159">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5bdad-160">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-160">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-161">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-161">Role</span></span>

* <span data-ttu-id="5bdad-162">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="5bdad-162">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-163">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-163">SQL</span></span>

* <span data-ttu-id="5bdad-164">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-164">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-165">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-165">Storage</span></span>

* <span data-ttu-id="5bdad-166">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="5bdad-166">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-167">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-167">VM</span></span>

* <span data-ttu-id="5bdad-168">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="5bdad-168">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5bdad-169">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-169">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5bdad-170">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-170">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5bdad-171">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="5bdad-171">June 13, 2018</span></span>

<span data-ttu-id="5bdad-172">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5bdad-172">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-173">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-173">Core</span></span>

* <span data-ttu-id="5bdad-174">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="5bdad-174">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5bdad-175">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="5bdad-175">June 13, 2018</span></span>

<span data-ttu-id="5bdad-176">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5bdad-176">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5bdad-177">AKS</span><span class="sxs-lookup"><span data-stu-id="5bdad-177">AKS</span></span>

* <span data-ttu-id="5bdad-178">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-178">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5bdad-179">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="5bdad-179">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="5bdad-180">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-180">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5bdad-181">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-181">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5bdad-182">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-182">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-183">AppService</span><span class="sxs-lookup"><span data-stu-id="5bdad-183">AppService</span></span>

* <span data-ttu-id="5bdad-184">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-184">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5bdad-185">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="5bdad-185">June 5, 2018</span></span>

<span data-ttu-id="5bdad-186">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5bdad-186">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-187">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-187">Interactive</span></span>

* <span data-ttu-id="5bdad-188">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="5bdad-188">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5bdad-189">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="5bdad-189">June 5, 2018</span></span>

<span data-ttu-id="5bdad-190">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5bdad-190">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-191">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-191">Core</span></span>

* <span data-ttu-id="5bdad-192">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-192">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5bdad-193">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-193">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-194">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-194">ACR</span></span>

* <span data-ttu-id="5bdad-195">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-195">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5bdad-196">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-196">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5bdad-197">AKS</span><span class="sxs-lookup"><span data-stu-id="5bdad-197">AKS</span></span>

* <span data-ttu-id="5bdad-198">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-198">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-199">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-199">Batch</span></span>

* <span data-ttu-id="5bdad-200">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5bdad-200">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-201">IOT</span><span class="sxs-lookup"><span data-stu-id="5bdad-201">IOT</span></span>

* <span data-ttu-id="5bdad-202">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-202">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-203">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-203">Network</span></span>

* <span data-ttu-id="5bdad-204">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="5bdad-204">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5bdad-205">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="5bdad-205">Policy Insights</span></span>

* <span data-ttu-id="5bdad-206">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-206">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5bdad-207">ARM</span><span class="sxs-lookup"><span data-stu-id="5bdad-207">ARM</span></span>

* <span data-ttu-id="5bdad-208">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-208">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-209">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-209">SQL</span></span>

* <span data-ttu-id="5bdad-210">관리형 새 인스턴스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-210">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5bdad-211">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-211">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5bdad-212">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-212">Storage</span></span>

* <span data-ttu-id="5bdad-213">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="5bdad-213">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-214">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-214">VM</span></span>

* <span data-ttu-id="5bdad-215">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-215">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5bdad-216">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-216">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5bdad-217">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-217">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5bdad-218">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="5bdad-218">May 22, 2018</span></span>

<span data-ttu-id="5bdad-219">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5bdad-219">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-220">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-220">Core</span></span>

* <span data-ttu-id="5bdad-221">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-221">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-222">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-222">ACS</span></span>

* <span data-ttu-id="5bdad-223">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-223">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5bdad-224">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-224">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-225">AppService</span><span class="sxs-lookup"><span data-stu-id="5bdad-225">AppService</span></span>

* <span data-ttu-id="5bdad-226">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-226">Improved generic update commands</span></span>
* <span data-ttu-id="5bdad-227">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-227">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-228">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-228">Container</span></span>

* <span data-ttu-id="5bdad-229">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-229">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5bdad-230">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-230">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-231">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-231">Extension</span></span>

* <span data-ttu-id="5bdad-232">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-232">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-233">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-233">Interactive</span></span>

* <span data-ttu-id="5bdad-234">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-234">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5bdad-235">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="5bdad-235">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-236">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bdad-236">KeyVault</span></span>

* <span data-ttu-id="5bdad-237">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="5bdad-237">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-238">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-238">Network</span></span>

* <span data-ttu-id="5bdad-239">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="5bdad-239">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5bdad-240">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-240">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-241">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-241">SQL</span></span>

* <span data-ttu-id="5bdad-242">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="5bdad-242">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5bdad-243">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="5bdad-243">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5bdad-244">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-244">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="5bdad-245">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-245">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5bdad-246">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-246">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5bdad-247">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="5bdad-247">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5bdad-248">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-248">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5bdad-249">`edition`</span><span class="sxs-lookup"><span data-stu-id="5bdad-249">`edition`.</span></span> <span data-ttu-id="5bdad-250">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-250">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5bdad-251">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="5bdad-251">`elasticPoolName`.</span></span> <span data-ttu-id="5bdad-252">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-252">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5bdad-253">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-253">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5bdad-254">`edition`</span><span class="sxs-lookup"><span data-stu-id="5bdad-254">`edition`.</span></span> <span data-ttu-id="5bdad-255">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="5bdad-255">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5bdad-256">`dtu`</span><span class="sxs-lookup"><span data-stu-id="5bdad-256">`dtu`.</span></span> <span data-ttu-id="5bdad-257">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="5bdad-257">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5bdad-258">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="5bdad-258">`databaseDtuMin`.</span></span> <span data-ttu-id="5bdad-259">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="5bdad-259">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5bdad-260">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="5bdad-260">`databaseDtuMax`.</span></span> <span data-ttu-id="5bdad-261">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="5bdad-261">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5bdad-262">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-262">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5bdad-263">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-263">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-264">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-264">Storage</span></span>

* <span data-ttu-id="5bdad-265">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-265">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5bdad-266">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-266">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-267">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-267">VM</span></span>

* <span data-ttu-id="5bdad-268">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="5bdad-268">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5bdad-269">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="5bdad-269">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5bdad-270">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="5bdad-270">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5bdad-271">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="5bdad-271">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5bdad-272">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-272">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5bdad-273">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="5bdad-273">May 7, 2018</span></span>

<span data-ttu-id="5bdad-274">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5bdad-274">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-275">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-275">Core</span></span>

* <span data-ttu-id="5bdad-276">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-276">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5bdad-277">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-277">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5bdad-278">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-278">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5bdad-279">#5591</span><span class="sxs-lookup"><span data-stu-id="5bdad-279">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5bdad-280">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-280">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5bdad-281">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-281">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5bdad-282">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-282">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5bdad-283">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-283">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5bdad-284">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-284">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-285">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-285">ACR</span></span>

* <span data-ttu-id="5bdad-286">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-286">Added ACR Build commands</span></span>
* <span data-ttu-id="5bdad-287">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-287">Improved resource not found error messages</span></span>
* <span data-ttu-id="5bdad-288">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-288">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5bdad-289">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-289">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5bdad-290">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-290">Improved repository commands error messages</span></span>
* <span data-ttu-id="5bdad-291">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="5bdad-291">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-292">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-292">ACS</span></span>

* <span data-ttu-id="5bdad-293">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-293">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5bdad-294">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-294">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5bdad-295">AMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-295">AMS</span></span>

* <span data-ttu-id="5bdad-296">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="5bdad-296">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-297">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-297">Appservice</span></span>

* <span data-ttu-id="5bdad-298">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-298">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5bdad-299">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-299">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5bdad-300">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-300">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5bdad-301">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-301">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bdad-302">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5bdad-302">Batch AI</span></span>

* <span data-ttu-id="5bdad-303">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-303">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bdad-304">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5bdad-304">Cognitive Services</span></span>

* <span data-ttu-id="5bdad-305">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-305">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5bdad-306">Consumption</span><span class="sxs-lookup"><span data-stu-id="5bdad-306">Consumption</span></span>

* <span data-ttu-id="5bdad-307">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-307">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-308">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-308">Container</span></span>

* <span data-ttu-id="5bdad-309">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-309">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5bdad-310">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bdad-310">Cosmos DB</span></span>

* <span data-ttu-id="5bdad-311">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bdad-311">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5bdad-312">DMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-312">DMS</span></span>

* <span data-ttu-id="5bdad-313">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-313">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-314">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-314">Extension</span></span>

* <span data-ttu-id="5bdad-315">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-315">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-316">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-316">Interactive</span></span>

* <span data-ttu-id="5bdad-317">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-317">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5bdad-318">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="5bdad-318">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5bdad-319">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-319">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5bdad-320">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-320">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5bdad-321">랩</span><span class="sxs-lookup"><span data-stu-id="5bdad-321">Lab</span></span>

* <span data-ttu-id="5bdad-322">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-322">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-323">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-323">Network</span></span>

* <span data-ttu-id="5bdad-324">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-324">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5bdad-325">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-325">Profile</span></span>

* <span data-ttu-id="5bdad-326">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-326">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5bdad-327">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-327">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5bdad-328">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-328">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5bdad-329">Redis</span><span class="sxs-lookup"><span data-stu-id="5bdad-329">Redis</span></span>

* <span data-ttu-id="5bdad-330">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-330">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5bdad-331">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-331">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5bdad-332">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-332">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5bdad-333">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-333">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5bdad-334">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-334">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-335">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-335">Role</span></span>

* <span data-ttu-id="5bdad-336">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-336">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-337">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-337">Storage</span></span>

* <span data-ttu-id="5bdad-338">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-338">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5bdad-339">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="5bdad-339">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5bdad-340">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="5bdad-340">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5bdad-341">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-341">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5bdad-342">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-342">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-343">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-343">VM</span></span>

* <span data-ttu-id="5bdad-344">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-344">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5bdad-345">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-345">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5bdad-346">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="5bdad-346">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5bdad-347">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-347">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5bdad-348">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-348">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5bdad-349">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-349">Added write accelerator support</span></span> 
* <span data-ttu-id="5bdad-350">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-350">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5bdad-351">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-351">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5bdad-352">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-352">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5bdad-353">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="5bdad-353">April 10, 2018</span></span>

<span data-ttu-id="5bdad-354">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5bdad-354">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-355">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-355">ACR</span></span>

* <span data-ttu-id="5bdad-356">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="5bdad-356">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-357">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-357">ACS</span></span>

* <span data-ttu-id="5bdad-358">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-358">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-359">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-359">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5bdad-361">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-361">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5bdad-362">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5bdad-362">BatchAI</span></span>

* <span data-ttu-id="5bdad-363">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-363">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="5bdad-364">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="5bdad-364">Job level mounting</span></span>
 - <span data-ttu-id="5bdad-365">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="5bdad-365">Environment variables with secret values</span></span>
 - <span data-ttu-id="5bdad-366">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-366">Performance counters settings</span></span>
 - <span data-ttu-id="5bdad-367">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="5bdad-367">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="5bdad-368">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-368">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="5bdad-369">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="5bdad-369">Usage and limits reporting</span></span>
 - <span data-ttu-id="5bdad-370">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-370">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="5bdad-371">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-371">Support for custom images</span></span>
 - <span data-ttu-id="5bdad-372">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-372">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5bdad-373">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-373">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5bdad-374">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-374">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5bdad-375">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-375">National clouds are supported</span></span>
* <span data-ttu-id="5bdad-376">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-376">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5bdad-377">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="5bdad-377">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5bdad-378">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-378">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5bdad-379">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-379">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5bdad-380">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="5bdad-380">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5bdad-381">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="5bdad-381">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5bdad-382">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-382">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5bdad-383">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-383">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5bdad-384">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-384">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5bdad-385">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-385">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5bdad-386">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-386">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5bdad-387">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="5bdad-387">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5bdad-388">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-388">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5bdad-389">결제</span><span class="sxs-lookup"><span data-stu-id="5bdad-389">Billing</span></span>

* <span data-ttu-id="5bdad-390">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-390">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5bdad-391">Consumption</span><span class="sxs-lookup"><span data-stu-id="5bdad-391">Consumption</span></span>

* <span data-ttu-id="5bdad-392">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-392">Added `marketplace` commands</span></span>
* <span data-ttu-id="5bdad-393">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-393">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5bdad-394">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-394">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5bdad-395">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-395">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5bdad-396">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-396">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5bdad-397">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-397">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-398">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-398">Container</span></span>

* <span data-ttu-id="5bdad-399">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="5bdad-399">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5bdad-400">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="5bdad-400">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-401">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-401">Extension</span></span>

* <span data-ttu-id="5bdad-402">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-402">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-403">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-403">Interactive</span></span>

* <span data-ttu-id="5bdad-404">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-404">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5bdad-405">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-405">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5bdad-406">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-406">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-407">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-407">Network</span></span>

* <span data-ttu-id="5bdad-408">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-408">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5bdad-409">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-409">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="5bdad-410">#4910</span><span class="sxs-lookup"><span data-stu-id="5bdad-410">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="5bdad-411">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-411">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="5bdad-412">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="5bdad-412">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5bdad-413">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-413">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5bdad-414">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-414">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5bdad-415">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-415">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-416">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-416">Profile</span></span>

* <span data-ttu-id="5bdad-417">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-417">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5bdad-418">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-418">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bdad-419">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-419">RDBMS</span></span>

* <span data-ttu-id="5bdad-420">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-420">Added `georestore` command</span></span>
* <span data-ttu-id="5bdad-421">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-421">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-422">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-422">Resource</span></span>

* <span data-ttu-id="5bdad-423">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-423">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5bdad-424">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-424">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-425">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-425">SQL</span></span>

* <span data-ttu-id="5bdad-426">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-426">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-427">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-427">Storage</span></span>

* <span data-ttu-id="5bdad-428">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-428">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-429">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-429">VM</span></span>

* <span data-ttu-id="5bdad-430">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-430">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5bdad-431">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-431">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="5bdad-433">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-433">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5bdad-434">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-434">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="5bdad-435">#5718</span><span class="sxs-lookup"><span data-stu-id="5bdad-435">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="5bdad-436">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-436">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5bdad-437">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="5bdad-437">March 27, 2018</span></span>

<span data-ttu-id="5bdad-438">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5bdad-438">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-439">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-439">Core</span></span>

* <span data-ttu-id="5bdad-440">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="5bdad-440">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-441">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-441">ACS</span></span>

* <span data-ttu-id="5bdad-442">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-442">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-443">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-443">Appservice</span></span>

* <span data-ttu-id="5bdad-444">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-444">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5bdad-445">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-445">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5bdad-446">Backup</span><span class="sxs-lookup"><span data-stu-id="5bdad-446">Backup</span></span>

* <span data-ttu-id="5bdad-447">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-447">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5bdad-448">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-448">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5bdad-449">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-449">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5bdad-450">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-450">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-451">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-451">Container</span></span>

* <span data-ttu-id="5bdad-452">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-452">Added `container exec` command.</span></span> <span data-ttu-id="5bdad-453">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-453">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5bdad-454">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-454">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-455">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-455">Extension</span></span>

* <span data-ttu-id="5bdad-456">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-456">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5bdad-457">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-457">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5bdad-458">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-458">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-459">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-459">Interactive</span></span>

* <span data-ttu-id="5bdad-460">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="5bdad-460">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5bdad-461">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-461">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5bdad-462">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-462">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5bdad-463">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-463">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5bdad-464">랩</span><span class="sxs-lookup"><span data-stu-id="5bdad-464">Lab</span></span>

* <span data-ttu-id="5bdad-465">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-465">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-466">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-466">Monitor</span></span>

* <span data-ttu-id="5bdad-467">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-467">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5bdad-468">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="5bdad-468">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5bdad-469">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-469">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-470">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-470">Network</span></span>

* <span data-ttu-id="5bdad-471">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-471">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-472">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-472">Profile</span></span>

* <span data-ttu-id="5bdad-473">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-473">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bdad-474">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-474">RDBMS</span></span>

* <span data-ttu-id="5bdad-475">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-475">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-476">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-476">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5bdad-478">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-478">Role</span></span>

* <span data-ttu-id="5bdad-479">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-479">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5bdad-480">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-480">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5bdad-481">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-481">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5bdad-482">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-482">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5bdad-483">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-483">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-484">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-484">Storage</span></span>

* <span data-ttu-id="5bdad-485">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-485">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5bdad-486">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="5bdad-486">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-487">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-487">VM</span></span>

* <span data-ttu-id="5bdad-488">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-488">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5bdad-489">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-489">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5bdad-490">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-490">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5bdad-491">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-491">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5bdad-492">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="5bdad-492">March 13, 2018</span></span>

<span data-ttu-id="5bdad-493">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5bdad-493">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-494">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-494">ACR</span></span>

* <span data-ttu-id="5bdad-495">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-495">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5bdad-496">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-496">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5bdad-497">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-497">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-498">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-498">ACS</span></span>

* <span data-ttu-id="5bdad-499">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-499">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5bdad-500">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-500">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5bdad-501">Advisor</span><span class="sxs-lookup"><span data-stu-id="5bdad-501">Advisor</span></span>

* <span data-ttu-id="5bdad-502">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-502">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5bdad-503">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-503">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5bdad-504">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-504">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="5bdad-505">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-505">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5bdad-506">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-506">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-507">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-507">Appservice</span></span>

* <span data-ttu-id="5bdad-508">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-508">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5bdad-509">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-509">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5bdad-510">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="5bdad-510">Eventhubs</span></span>

* <span data-ttu-id="5bdad-511">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-511">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-512">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-512">Extension</span></span>

* <span data-ttu-id="5bdad-513">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-513">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-514">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-514">Interactive</span></span>

* <span data-ttu-id="5bdad-515">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="5bdad-515">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5bdad-516">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="5bdad-516">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5bdad-517">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-517">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5bdad-518">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-518">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-519">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-519">Monitor</span></span>

* <span data-ttu-id="5bdad-520">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-520">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5bdad-521">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-521">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5bdad-522">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-522">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5bdad-523">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-523">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-524">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-524">Network</span></span>

* <span data-ttu-id="5bdad-525">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-525">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5bdad-526">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="5bdad-526">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5bdad-527">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-527">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5bdad-528">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-528">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-529">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-529">Profile</span></span>

* <span data-ttu-id="5bdad-530">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-530">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5bdad-531">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-531">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bdad-532">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-532">RDBMS</span></span>

* <span data-ttu-id="5bdad-533">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-533">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5bdad-534">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5bdad-534">Service Bus</span></span>

* <span data-ttu-id="5bdad-535">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-535">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-536">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-536">Storage</span></span>

* <span data-ttu-id="5bdad-537">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-537">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5bdad-538">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-538">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-539">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-539">VM</span></span>

* <span data-ttu-id="5bdad-540">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-540">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5bdad-541">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-541">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5bdad-542">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-542">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5bdad-543">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-543">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5bdad-544">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="5bdad-544">February 27, 2018</span></span>

<span data-ttu-id="5bdad-545">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5bdad-545">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-546">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-546">Core</span></span>

* <span data-ttu-id="5bdad-547">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-547">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5bdad-548">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-548">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5bdad-549">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-549">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-550">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-550">ACS</span></span>

* <span data-ttu-id="5bdad-551">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-551">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5bdad-552">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-552">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5bdad-553">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-553">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5bdad-554">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-554">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-555">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-555">Appservice</span></span>

* <span data-ttu-id="5bdad-556">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5bdad-556">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5bdad-557">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-557">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bdad-558">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5bdad-558">Cognitive Services</span></span>

* <span data-ttu-id="5bdad-559">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="5bdad-559">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5bdad-560">Consumption</span><span class="sxs-lookup"><span data-stu-id="5bdad-560">Consumption</span></span>

* <span data-ttu-id="5bdad-561">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-561">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5bdad-562">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="5bdad-562">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-563">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-563">Container</span></span>

* <span data-ttu-id="5bdad-564">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-564">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-565">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-565">Network</span></span>

* <span data-ttu-id="5bdad-566">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-566">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-567">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-567">Resource</span></span>

* <span data-ttu-id="5bdad-568">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-568">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-569">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-569">Role</span></span>

* <span data-ttu-id="5bdad-570">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-570">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-571">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-571">SQL</span></span>

* <span data-ttu-id="5bdad-572">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-572">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-573">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-573">Storage</span></span>

* <span data-ttu-id="5bdad-574">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="5bdad-574">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-575">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-575">VM</span></span>

* <span data-ttu-id="5bdad-576">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-576">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5bdad-577">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="5bdad-577">February 13, 2018</span></span>

<span data-ttu-id="5bdad-578">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5bdad-578">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-579">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-579">Core</span></span>

* <span data-ttu-id="5bdad-580">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-580">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-581">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-581">ACS</span></span>

* <span data-ttu-id="5bdad-582">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-582">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5bdad-583">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-583">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5bdad-584">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-584">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5bdad-585">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="5bdad-585">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5bdad-586">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-586">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5bdad-587">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="5bdad-587">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5bdad-588">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-588">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5bdad-589">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-589">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-590">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-590">Appservice</span></span>

* <span data-ttu-id="5bdad-591">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-591">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5bdad-592">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-592">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5bdad-593">CDN</span><span class="sxs-lookup"><span data-stu-id="5bdad-593">CDN</span></span>

* <span data-ttu-id="5bdad-594">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-594">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-595">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-595">Container</span></span>

* <span data-ttu-id="5bdad-596">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-596">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5bdad-597">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-597">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bdad-598">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bdad-598">CosmosDB</span></span>

* <span data-ttu-id="5bdad-599">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-599">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-600">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-600">Extension</span></span>

* <span data-ttu-id="5bdad-601">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-601">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5bdad-602">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-602">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5bdad-603">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="5bdad-603">Feedback</span></span>

* <span data-ttu-id="5bdad-604">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-604">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-605">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-605">Interactive</span></span>

* <span data-ttu-id="5bdad-606">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-606">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5bdad-607">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-607">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-608">IoT</span><span class="sxs-lookup"><span data-stu-id="5bdad-608">IoT</span></span>

* <span data-ttu-id="5bdad-609">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-609">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5bdad-610">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-610">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5bdad-611">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-611">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5bdad-612">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-612">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-613">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-613">Monitor</span></span>

* <span data-ttu-id="5bdad-614">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-614">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-615">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-615">Network</span></span>

* <span data-ttu-id="5bdad-616">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-616">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5bdad-617">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-617">Profile</span></span>

* <span data-ttu-id="5bdad-618">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-618">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-619">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-619">Resource</span></span>

* <span data-ttu-id="5bdad-620">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-620">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-621">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-621">Role</span></span>

* <span data-ttu-id="5bdad-622">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-622">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-623">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-623">SQL</span></span>

* <span data-ttu-id="5bdad-624">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-624">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5bdad-625">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-625">Added `sql db rename`</span></span>
* <span data-ttu-id="5bdad-626">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-626">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-627">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-627">Storage</span></span>

* <span data-ttu-id="5bdad-628">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-628">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-629">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-629">VM</span></span>

* <span data-ttu-id="5bdad-630">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-630">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5bdad-631">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-631">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5bdad-632">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="5bdad-632">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5bdad-633">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="5bdad-633">January 31, 2018</span></span>

<span data-ttu-id="5bdad-634">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5bdad-634">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-635">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-635">Core</span></span>

* <span data-ttu-id="5bdad-636">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-636">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5bdad-637">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-637">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5bdad-638">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-638">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5bdad-639">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="5bdad-639">Use `--verbose` to see</span></span>
* <span data-ttu-id="5bdad-640">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-640">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-641">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-641">ACS</span></span>

* <span data-ttu-id="5bdad-642">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-642">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5bdad-643">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="5bdad-643">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-644">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-644">Appservice</span></span>

* <span data-ttu-id="5bdad-645">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="5bdad-645">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5bdad-646">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-646">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5bdad-647">CDN</span><span class="sxs-lookup"><span data-stu-id="5bdad-647">CDN</span></span>

* <span data-ttu-id="5bdad-648">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-648">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bdad-649">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bdad-649">CosmosDB</span></span>

* <span data-ttu-id="5bdad-650">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-650">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-651">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-651">Interactive</span></span>

* <span data-ttu-id="5bdad-652">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-652">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-653">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-653">Network</span></span>

* <span data-ttu-id="5bdad-654">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-654">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5bdad-655">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-655">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5bdad-656">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-656">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5bdad-657">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-657">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5bdad-658">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-658">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5bdad-659">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="5bdad-659">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5bdad-660">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-660">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5bdad-661">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-661">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5bdad-662">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-662">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="5bdad-663">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="5bdad-663">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-664">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-664">Profile</span></span>

* <span data-ttu-id="5bdad-665">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-665">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-666">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-666">Resource</span></span>

* <span data-ttu-id="5bdad-667">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-667">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-668">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-668">Storage</span></span>

* <span data-ttu-id="5bdad-669">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-669">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5bdad-670">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-670">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5bdad-671">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-671">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="5bdad-672">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-672">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5bdad-673">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-673">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-674">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-674">VM</span></span>

* <span data-ttu-id="5bdad-675">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-675">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5bdad-676">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-676">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5bdad-677">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-677">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5bdad-678">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-678">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5bdad-679">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="5bdad-679">January 17, 2018</span></span>

<span data-ttu-id="5bdad-680">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5bdad-680">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-681">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-681">ACR</span></span>

* <span data-ttu-id="5bdad-682">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-682">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5bdad-683">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-683">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-684">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-684">ACS</span></span>

* <span data-ttu-id="5bdad-685">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-685">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5bdad-686">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-686">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-687">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-687">Appservice</span></span>

* <span data-ttu-id="5bdad-688">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-688">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5bdad-689">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-689">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5bdad-690">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-690">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5bdad-691">Backup</span><span class="sxs-lookup"><span data-stu-id="5bdad-691">Backup</span></span>

* <span data-ttu-id="5bdad-692">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-692">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5bdad-693">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-693">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5bdad-694">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-694">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5bdad-695">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-695">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5bdad-696">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-696">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-697">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-697">Batch</span></span>

* <span data-ttu-id="5bdad-698">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-698">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5bdad-699">클라우드</span><span class="sxs-lookup"><span data-stu-id="5bdad-699">Cloud</span></span>

* <span data-ttu-id="5bdad-700">클라우드에서 `--profile`을 설정할 때 끝점을 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-700">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5bdad-701">Consumption</span><span class="sxs-lookup"><span data-stu-id="5bdad-701">Consumption</span></span>

* <span data-ttu-id="5bdad-702">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-702">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bdad-703">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5bdad-703">Event Grid</span></span>

* <span data-ttu-id="5bdad-704">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-704">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5bdad-705">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-705">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5bdad-706">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-706">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5bdad-707">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="5bdad-707">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5bdad-708">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-708">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5bdad-709">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-709">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5bdad-710">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-710">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5bdad-711">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-711">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-712">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-712">Interactive</span></span>

* <span data-ttu-id="5bdad-713">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-713">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5bdad-714">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-714">Fixed errors on startup</span></span>
* <span data-ttu-id="5bdad-715">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-715">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-716">IoT</span><span class="sxs-lookup"><span data-stu-id="5bdad-716">IoT</span></span>

* <span data-ttu-id="5bdad-717">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-717">Added support for device provisioning service</span></span>
* <span data-ttu-id="5bdad-718">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-718">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5bdad-719">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-719">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-720">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-720">Monitor</span></span>

* <span data-ttu-id="5bdad-721">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-721">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5bdad-722">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="5bdad-722">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5bdad-723">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-723">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-724">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-724">Network</span></span>

* <span data-ttu-id="5bdad-725">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-725">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5bdad-726">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-726">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-727">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-727">Profile</span></span>

* <span data-ttu-id="5bdad-728">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-728">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-729">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-729">Role</span></span>

* <span data-ttu-id="5bdad-730">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-730">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bdad-731">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bdad-731">Service Fabric</span></span>

* <span data-ttu-id="5bdad-732">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-732">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5bdad-733">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-733">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-734">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-734">VM</span></span>

* <span data-ttu-id="5bdad-735">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-735">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5bdad-736">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-736">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5bdad-737">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-737">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5bdad-738">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-738">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5bdad-739">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-739">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5bdad-740">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-740">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bdad-741">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-741">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bdad-742">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-742">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5bdad-743">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="5bdad-743">December 19, 2017</span></span>

<span data-ttu-id="5bdad-744">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5bdad-744">Version 2.0.23</span></span>

* <span data-ttu-id="5bdad-745">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-745">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-746">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-746">Container</span></span>

* <span data-ttu-id="5bdad-747">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-747">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-748">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-748">Network</span></span>

* <span data-ttu-id="5bdad-749">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-749">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5bdad-750">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-750">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-751">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-751">Storage</span></span>

* <span data-ttu-id="5bdad-752">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-752">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-753">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-753">VM</span></span>

* <span data-ttu-id="5bdad-754">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-754">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5bdad-755">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="5bdad-755">December 5, 2017</span></span>

<span data-ttu-id="5bdad-756">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5bdad-756">Version 2.0.22</span></span>

* <span data-ttu-id="5bdad-757">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-757">Removed `az component` commands.</span></span> <span data-ttu-id="5bdad-758">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="5bdad-758">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-759">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-759">Core</span></span>
* <span data-ttu-id="5bdad-760">`AZURE_US_GOV_CLOUD` AAD 권한 끝점이 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-760">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5bdad-761">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-761">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-762">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-762">ACS</span></span>

* <span data-ttu-id="5bdad-763">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-763">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5bdad-764">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-764">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5bdad-765">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-765">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5bdad-766">Advisor</span><span class="sxs-lookup"><span data-stu-id="5bdad-766">Advisor</span></span>

* <span data-ttu-id="5bdad-767">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-767">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-768">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-768">Appservice</span></span>

* <span data-ttu-id="5bdad-769">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-769">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5bdad-770">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-770">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5bdad-771">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-771">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5bdad-772">Consumption</span><span class="sxs-lookup"><span data-stu-id="5bdad-772">Consumption</span></span>

* <span data-ttu-id="5bdad-773">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-773">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-774">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-774">Container</span></span>

* <span data-ttu-id="5bdad-775">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-775">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-776">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-776">Monitor</span></span>

* <span data-ttu-id="5bdad-777">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-777">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-778">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-778">Resource</span></span>

* <span data-ttu-id="5bdad-779">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-779">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-780">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-780">Role</span></span>

* <span data-ttu-id="5bdad-781">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-781">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5bdad-782">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-782">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5bdad-783">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-783">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-784">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-784">SQL</span></span>

* <span data-ttu-id="5bdad-785">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-785">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5bdad-786">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-786">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-787">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-787">VM</span></span>

* <span data-ttu-id="5bdad-788">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-788">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5bdad-789">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="5bdad-789">November 14, 2017</span></span>

<span data-ttu-id="5bdad-790">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5bdad-790">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-791">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-791">ACR</span></span>

* <span data-ttu-id="5bdad-792">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-792">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5bdad-793">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-793">ACS</span></span>

* <span data-ttu-id="5bdad-794">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-794">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5bdad-795">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="5bdad-795">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5bdad-796">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-796">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5bdad-797">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-797">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5bdad-798">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-798">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-799">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-799">Appservice</span></span>

* <span data-ttu-id="5bdad-800">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-800">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5bdad-801">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-801">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5bdad-802">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-802">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5bdad-803">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-803">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5bdad-804">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-804">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5bdad-805">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="5bdad-805">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-806">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-806">Batch</span></span>

* <span data-ttu-id="5bdad-807">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-807">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5bdad-808">Batchai</span><span class="sxs-lookup"><span data-stu-id="5bdad-808">Batchai</span></span>

* <span data-ttu-id="5bdad-809">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-809">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5bdad-810">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-810">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5bdad-811">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-811">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5bdad-812">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-812">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5bdad-813">클라우드</span><span class="sxs-lookup"><span data-stu-id="5bdad-813">Cloud</span></span>

* <span data-ttu-id="5bdad-814">필요한 끝점이 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-814">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-815">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-815">Container</span></span>

* <span data-ttu-id="5bdad-816">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-816">Added support to open multiple ports</span></span>
* <span data-ttu-id="5bdad-817">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-817">Added container group restart policy</span></span>
* <span data-ttu-id="5bdad-818">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-818">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5bdad-819">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="5bdad-819">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bdad-820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bdad-820">Data Lake Analytics</span></span>

* <span data-ttu-id="5bdad-821">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-821">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bdad-822">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bdad-822">Data Lake Store</span></span>

* <span data-ttu-id="5bdad-823">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-823">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-824">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-824">Extension</span></span>

* <span data-ttu-id="5bdad-825">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-825">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5bdad-826">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-826">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-827">IoT</span><span class="sxs-lookup"><span data-stu-id="5bdad-827">IoT</span></span>

* <span data-ttu-id="5bdad-828">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-828">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-829">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-829">Monitor</span></span>

* <span data-ttu-id="5bdad-830">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-830">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-831">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-831">Network</span></span>

* <span data-ttu-id="5bdad-832">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-832">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5bdad-833">`traffic-manager profile update`로 끝점을 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-833">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5bdad-834">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-834">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5bdad-835">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-835">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5bdad-836">예약</span><span class="sxs-lookup"><span data-stu-id="5bdad-836">Reservations</span></span>

* <span data-ttu-id="5bdad-837">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-837">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-838">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-838">Resource</span></span>

* <span data-ttu-id="5bdad-839">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-839">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-840">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-840">SQL</span></span>

* <span data-ttu-id="5bdad-841">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-841">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-842">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-842">Storage</span></span>

* <span data-ttu-id="5bdad-843">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-843">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5bdad-844">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-844">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5bdad-845">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-845">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5bdad-846">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="5bdad-846">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5bdad-847">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-847">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5bdad-848">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-848">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5bdad-849">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-849">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-850">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-850">VM</span></span>

* <span data-ttu-id="5bdad-851">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-851">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5bdad-852">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-852">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5bdad-853">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-853">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5bdad-854">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-854">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5bdad-855">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-855">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5bdad-856">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="5bdad-856">October 24, 2017</span></span>

<span data-ttu-id="5bdad-857">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5bdad-857">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-858">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-858">Core</span></span>

* <span data-ttu-id="5bdad-859">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="5bdad-859">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-860">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-860">ACR</span></span>

* <span data-ttu-id="5bdad-861">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="5bdad-861">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5bdad-862">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-862">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5bdad-863">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="5bdad-863">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-864">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-864">ACS</span></span>

* <span data-ttu-id="5bdad-865">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-865">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5bdad-866">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-866">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-867">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-867">Appservice</span></span>

* <span data-ttu-id="5bdad-868">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-868">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5bdad-869">구성 요소</span><span class="sxs-lookup"><span data-stu-id="5bdad-869">Component</span></span>

* <span data-ttu-id="5bdad-870">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-870">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-871">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-871">Monitor</span></span>

* <span data-ttu-id="5bdad-872">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-872">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-873">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-873">Resource</span></span>

* <span data-ttu-id="5bdad-874">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-874">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5bdad-875">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-875">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-876">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-876">VM</span></span>

* <span data-ttu-id="5bdad-877">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-877">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5bdad-878">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="5bdad-878">October 9, 2017</span></span>

<span data-ttu-id="5bdad-879">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5bdad-879">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-880">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-880">Core</span></span>

* <span data-ttu-id="5bdad-881">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-881">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-882">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-882">Appservice</span></span>

* <span data-ttu-id="5bdad-883">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-883">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-884">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-884">Batch</span></span>

* <span data-ttu-id="5bdad-885">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-885">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5bdad-886">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-886">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5bdad-887">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-887">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5bdad-888">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-888">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5bdad-889">Batchai</span><span class="sxs-lookup"><span data-stu-id="5bdad-889">Batchai</span></span>

* <span data-ttu-id="5bdad-890">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-890">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-891">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bdad-891">Keyvault</span></span>

* <span data-ttu-id="5bdad-892">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-892">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5bdad-893">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5bdad-893">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5bdad-894">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-894">Network</span></span>

* <span data-ttu-id="5bdad-895">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-895">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5bdad-896">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-896">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-897">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-897">Resource</span></span>

* <span data-ttu-id="5bdad-898">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-898">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5bdad-899">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-899">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5bdad-900">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-900">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5bdad-901">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-901">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-902">Sql</span><span class="sxs-lookup"><span data-stu-id="5bdad-902">Sql</span></span>

* <span data-ttu-id="5bdad-903">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-903">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5bdad-904">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-904">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5bdad-905">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-905">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-906">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-906">Storage</span></span>

* <span data-ttu-id="5bdad-907">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-907">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-908">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-908">Vm</span></span>

* <span data-ttu-id="5bdad-909">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-909">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5bdad-910">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-910">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5bdad-911">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-911">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5bdad-912">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-912">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5bdad-913">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-913">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5bdad-914">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="5bdad-914">September 22, 2017</span></span>

<span data-ttu-id="5bdad-915">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5bdad-915">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-916">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-916">Resource</span></span>

* <span data-ttu-id="5bdad-917">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-917">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5bdad-918">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-918">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5bdad-919">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-919">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5bdad-920">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-920">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-921">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-921">Network</span></span>

* <span data-ttu-id="5bdad-922">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-922">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5bdad-923">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-923">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5bdad-924">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-924">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5bdad-925">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-925">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5bdad-926">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-926">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5bdad-927">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-927">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5bdad-928">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-928">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-929">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-929">Storage</span></span>

* <span data-ttu-id="5bdad-930">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-930">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5bdad-931">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5bdad-931">Eventgrid</span></span>

* <span data-ttu-id="5bdad-932">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="5bdad-932">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-933">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-933">SQL</span></span>

* <span data-ttu-id="5bdad-934">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-934">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5bdad-935">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-935">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5bdad-936">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-936">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-937">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bdad-937">Keyvault</span></span>

* <span data-ttu-id="5bdad-938">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-938">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-939">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-939">VM</span></span>

* <span data-ttu-id="5bdad-940">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-940">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5bdad-941">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="5bdad-941">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5bdad-942">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-942">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5bdad-943">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-943">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5bdad-944">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-944">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5bdad-945">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-945">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-946">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-946">ACS</span></span>

* <span data-ttu-id="5bdad-947">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-947">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-948">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-948">Appservice</span></span>

* <span data-ttu-id="5bdad-949">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-949">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5bdad-950">Backup</span><span class="sxs-lookup"><span data-stu-id="5bdad-950">Backup</span></span>

* <span data-ttu-id="5bdad-951">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-951">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5bdad-952">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="5bdad-952">September 11, 2017</span></span>

<span data-ttu-id="5bdad-953">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5bdad-953">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5bdad-954">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-954">Core</span></span>

* <span data-ttu-id="5bdad-955">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-955">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5bdad-956">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-956">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-957">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-957">Acs</span></span>

* <span data-ttu-id="5bdad-958">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-958">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5bdad-959">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="5bdad-959">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-960">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-960">Appservice</span></span>

* <span data-ttu-id="5bdad-961">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-961">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5bdad-962">CDN</span><span class="sxs-lookup"><span data-stu-id="5bdad-962">CDN</span></span>

* <span data-ttu-id="5bdad-963">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-963">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5bdad-964">내선 번호</span><span class="sxs-lookup"><span data-stu-id="5bdad-964">Extension</span></span>

* <span data-ttu-id="5bdad-965">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-965">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-966">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bdad-966">Keyvault</span></span>

* <span data-ttu-id="5bdad-967">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-967">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-968">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-968">Network</span></span>

* <span data-ttu-id="5bdad-969">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-969">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5bdad-970">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-970">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5bdad-971">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-971">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5bdad-972">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-972">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5bdad-973">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-973">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-974">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-974">Resource</span></span>

* <span data-ttu-id="5bdad-975">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-975">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5bdad-976">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-976">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5bdad-977">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-977">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5bdad-978">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="5bdad-978">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-979">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-979">SQL</span></span>

* <span data-ttu-id="5bdad-980">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-980">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-981">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-981">VM</span></span>

* <span data-ttu-id="5bdad-982">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-982">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5bdad-983">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="5bdad-983">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5bdad-984">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-984">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5bdad-985">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-985">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5bdad-986">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-986">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5bdad-987">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="5bdad-987">August 31, 2017</span></span>

<span data-ttu-id="5bdad-988">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5bdad-988">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-989">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bdad-989">Keyvault</span></span>

* <span data-ttu-id="5bdad-990">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-990">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5bdad-991">Sf</span><span class="sxs-lookup"><span data-stu-id="5bdad-991">Sf</span></span>

* <span data-ttu-id="5bdad-992">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-992">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-993">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-993">Storage</span></span>

* <span data-ttu-id="5bdad-994">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-994">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5bdad-995">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="5bdad-995">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5bdad-996">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="5bdad-996">August 28, 2017</span></span>

<span data-ttu-id="5bdad-997">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5bdad-997">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5bdad-998">CLI</span><span class="sxs-lookup"><span data-stu-id="5bdad-998">CLI</span></span>

* <span data-ttu-id="5bdad-999">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-999">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1000">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1000">ACS</span></span>

* <span data-ttu-id="5bdad-1001">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1001">Corrected preview regions</span></span>
* <span data-ttu-id="5bdad-1002">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1002">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5bdad-1003">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1003">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-1004">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-1004">Appservice</span></span>

* <span data-ttu-id="5bdad-1005">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1005">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5bdad-1006">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1006">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5bdad-1007">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1007">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5bdad-1008">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1008">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5bdad-1009">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1009">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-1010">IoT</span><span class="sxs-lookup"><span data-stu-id="5bdad-1010">IoT</span></span>

* <span data-ttu-id="5bdad-1011">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1011">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-1012">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-1012">Network</span></span>

* <span data-ttu-id="5bdad-1013">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1013">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5bdad-1014">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1014">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5bdad-1015">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1015">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5bdad-1016">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1016">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5bdad-1017">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1017">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-1018">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-1018">Profile</span></span>

* <span data-ttu-id="5bdad-1019">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1019">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bdad-1020">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bdad-1020">Service Fabric</span></span>

* <span data-ttu-id="5bdad-1021">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1021">Preview release</span></span>
* <span data-ttu-id="5bdad-1022">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1022">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5bdad-1023">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1023">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5bdad-1024">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1024">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-1025">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-1025">Storage</span></span>

* <span data-ttu-id="5bdad-1026">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1026">Enabled setting blob tier</span></span>
* <span data-ttu-id="5bdad-1027">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1027">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5bdad-1028">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1028">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5bdad-1029">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1029">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5bdad-1030">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1030">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5bdad-1031">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1031">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-1032">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-1032">VM</span></span>

* <span data-ttu-id="5bdad-1033">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1033">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5bdad-1034">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1034">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5bdad-1035">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1035">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bdad-1036">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1036">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5bdad-1037">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1037">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5bdad-1038">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1038">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5bdad-1039">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1039">August 15, 2017</span></span>

<span data-ttu-id="5bdad-1040">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5bdad-1040">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1041">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1041">ACS</span></span>

* <span data-ttu-id="5bdad-1042">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1042">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-1043">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-1043">Appservice</span></span>

* <span data-ttu-id="5bdad-1044">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1044">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bdad-1045">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5bdad-1045">Event Grid</span></span>

* <span data-ttu-id="5bdad-1046">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1046">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5bdad-1047">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1047">August 11, 2017</span></span>

<span data-ttu-id="5bdad-1048">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5bdad-1048">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1049">ACS</span></span>

* <span data-ttu-id="5bdad-1050">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1050">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-1051">Batch</span></span>

* <span data-ttu-id="5bdad-1052">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1052">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5bdad-1053">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1053">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5bdad-1054">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1054">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5bdad-1055">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1055">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5bdad-1056">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1056">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5bdad-1057">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1057">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5bdad-1058">구성 요소</span><span class="sxs-lookup"><span data-stu-id="5bdad-1058">Component</span></span>

* <span data-ttu-id="5bdad-1059">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1059">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5bdad-1060">컨테이너</span><span class="sxs-lookup"><span data-stu-id="5bdad-1060">Container</span></span>

* <span data-ttu-id="5bdad-1061">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1061">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5bdad-1062">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bdad-1062">Data Lake Store</span></span>

* <span data-ttu-id="5bdad-1063">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1063">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bdad-1064">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5bdad-1064">Event Grid</span></span>

* <span data-ttu-id="5bdad-1065">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1065">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-1066">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-1066">Network</span></span>

* <span data-ttu-id="5bdad-1067">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1067">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5bdad-1068">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1068">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5bdad-1069">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1069">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5bdad-1070">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1070">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-1071">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-1071">Profile</span></span>

* <span data-ttu-id="5bdad-1072">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1072">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-1073">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-1073">Storage</span></span>

* <span data-ttu-id="5bdad-1074">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1074">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-1075">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-1075">VM</span></span>

* <span data-ttu-id="5bdad-1076">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1076">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5bdad-1077">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1077">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5bdad-1078">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1078">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5bdad-1079">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1079">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5bdad-1080">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1080">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5bdad-1081">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1081">July 28, 2017</span></span>

<span data-ttu-id="5bdad-1082">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5bdad-1082">Version 2.0.12</span></span>

* <span data-ttu-id="5bdad-1083">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1083">Added container commands</span></span>
* <span data-ttu-id="5bdad-1084">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1084">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5bdad-1085">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-1085">Core</span></span>

* <span data-ttu-id="5bdad-1086">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1086">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5bdad-1087">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1087">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5bdad-1088">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1088">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5bdad-1089">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1089">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5bdad-1090">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="5bdad-1090">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5bdad-1091">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1091">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5bdad-1092">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1092">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5bdad-1093">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1093">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5bdad-1094">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1094">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5bdad-1095">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1095">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5bdad-1096">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="5bdad-1096">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5bdad-1097">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1097">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5bdad-1098">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1098">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5bdad-1099">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1099">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5bdad-1100">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1100">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5bdad-1101">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1101">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5bdad-1102">ACR</span><span class="sxs-lookup"><span data-stu-id="5bdad-1102">ACR</span></span>

* <span data-ttu-id="5bdad-1103">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1103">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5bdad-1104">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1104">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5bdad-1105">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1105">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5bdad-1106">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1106">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5bdad-1107">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1107">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5bdad-1108">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1108">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1109">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1109">ACS</span></span>

* <span data-ttu-id="5bdad-1110">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1110">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-1111">App Service</span><span class="sxs-lookup"><span data-stu-id="5bdad-1111">Appservice</span></span>

* <span data-ttu-id="5bdad-1112">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1112">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5bdad-1113">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1113">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5bdad-1114">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1114">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5bdad-1115">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1115">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5bdad-1116">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1116">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5bdad-1117">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1117">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5bdad-1118">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1118">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5bdad-1119">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1119">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5bdad-1120">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1120">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5bdad-1121">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1121">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5bdad-1122">Batch</span><span class="sxs-lookup"><span data-stu-id="5bdad-1122">Batch</span></span>

* <span data-ttu-id="5bdad-1123">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1123">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5bdad-1124">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1124">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5bdad-1125">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1125">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5bdad-1126">CDN</span><span class="sxs-lookup"><span data-stu-id="5bdad-1126">CDN</span></span>

* <span data-ttu-id="5bdad-1127">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1127">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5bdad-1128">클라우드</span><span class="sxs-lookup"><span data-stu-id="5bdad-1128">Cloud</span></span>

* <span data-ttu-id="5bdad-1129">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1129">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5bdad-1130">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1130">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5bdad-1131">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1131">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5bdad-1132">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1132">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5bdad-1133">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1133">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bdad-1134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bdad-1134">CosmosDB</span></span>

* <span data-ttu-id="5bdad-1135">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1135">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5bdad-1136">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1136">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bdad-1137">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bdad-1137">Data Lake Analytics</span></span>

* <span data-ttu-id="5bdad-1138">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1138">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5bdad-1139">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1139">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5bdad-1140">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1140">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bdad-1141">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bdad-1141">Data Lake Store</span></span>

* <span data-ttu-id="5bdad-1142">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1142">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5bdad-1143">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1143">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5bdad-1144">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1144">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5bdad-1145">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="5bdad-1145">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5bdad-1146">대화형</span><span class="sxs-lookup"><span data-stu-id="5bdad-1146">Interactive</span></span>

* <span data-ttu-id="5bdad-1147">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1147">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5bdad-1148">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1148">Increased test coverage</span></span>
* <span data-ttu-id="5bdad-1149">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1149">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5bdad-1150">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1150">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5bdad-1151">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1151">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5bdad-1152">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1152">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5bdad-1153">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1153">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5bdad-1154">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1154">Added `--progress` flag</span></span>
* <span data-ttu-id="5bdad-1155">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1155">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5bdad-1156">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1156">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5bdad-1157">IoT</span><span class="sxs-lookup"><span data-stu-id="5bdad-1157">IoT</span></span>

* <span data-ttu-id="5bdad-1158">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1158">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5bdad-1159">(#3934)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1159">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5bdad-1160">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1160">Key vault</span></span>

* <span data-ttu-id="5bdad-1161">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="5bdad-1161">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5bdad-1162">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1162">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5bdad-1163">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1163">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5bdad-1164">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1164">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5bdad-1165">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1165">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5bdad-1166">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1166">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5bdad-1167">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1167">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5bdad-1168">(#3307)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1168">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5bdad-1169">랩</span><span class="sxs-lookup"><span data-stu-id="5bdad-1169">Lab</span></span>

* <span data-ttu-id="5bdad-1170">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1170">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5bdad-1171">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1171">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-1172">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-1172">Monitor</span></span>

* <span data-ttu-id="5bdad-1173">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1173">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5bdad-1174">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1174">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5bdad-1175">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1175">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5bdad-1176">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1176">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5bdad-1177">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1177">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5bdad-1178">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="5bdad-1178">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5bdad-1179">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1179">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5bdad-1180">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1180">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5bdad-1181">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1181">`location` no longer required</span></span>
  * <span data-ttu-id="5bdad-1182">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1182">Add name and ID support for target</span></span>
  * <span data-ttu-id="5bdad-1183">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1183">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5bdad-1184">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1184">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5bdad-1185">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1185">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5bdad-1186">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1186">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5bdad-1187">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1187">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5bdad-1188">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1188">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-1189">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-1189">Network</span></span>

* <span data-ttu-id="5bdad-1190">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1190">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5bdad-1191">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1191">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5bdad-1192">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1192">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5bdad-1193">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1193">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5bdad-1194">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1194">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5bdad-1195">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1195">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5bdad-1196">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1196">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5bdad-1197">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1197">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5bdad-1198">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1198">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5bdad-1199">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1199">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5bdad-1200">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1200">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5bdad-1201">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1201">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5bdad-1202">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1202">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5bdad-1203">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5bdad-1203">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5bdad-1204">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1204">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5bdad-1205">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1205">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5bdad-1206">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1206">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5bdad-1207">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1207">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5bdad-1208">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1208">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5bdad-1209">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1209">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5bdad-1210">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1210">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5bdad-1211">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1211">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5bdad-1212">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1212">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5bdad-1213">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1213">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5bdad-1214">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1214">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5bdad-1215">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1215">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5bdad-1216">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1216">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-1217">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-1217">Profile</span></span>

* <span data-ttu-id="5bdad-1218">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1218">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5bdad-1219">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1219">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5bdad-1220">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1220">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5bdad-1221">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1221">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5bdad-1222">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1222">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bdad-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1223">RDBMS</span></span>

* <span data-ttu-id="5bdad-1224">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1224">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5bdad-1225">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1225">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5bdad-1226">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1226">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5bdad-1227">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1227">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-1228">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1228">Resource</span></span>

* <span data-ttu-id="5bdad-1229">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1229">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5bdad-1230">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1230">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5bdad-1231">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1231">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5bdad-1232">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1232">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5bdad-1233">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1233">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5bdad-1234">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1234">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5bdad-1235">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1235">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5bdad-1236">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1236">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-1237">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-1237">Role</span></span>

* <span data-ttu-id="5bdad-1238">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1238">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5bdad-1239">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1239">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5bdad-1240">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1240">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5bdad-1241">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1241">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5bdad-1242">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1242">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bdad-1243">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bdad-1243">Service Fabric</span></span>
* <span data-ttu-id="5bdad-1244">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="5bdad-1244">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5bdad-1245">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1245">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5bdad-1246">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1246">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-1247">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-1247">SQL</span></span>

* <span data-ttu-id="5bdad-1248">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1248">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5bdad-1249">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1249">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5bdad-1250">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1250">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-1251">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-1251">Storage</span></span>

* <span data-ttu-id="5bdad-1252">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1252">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5bdad-1253">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="5bdad-1253">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5bdad-1254">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1254">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5bdad-1255">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1255">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5bdad-1256">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1256">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5bdad-1257">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1257">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-1258">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-1258">VM</span></span>

* <span data-ttu-id="5bdad-1259">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1259">Support configuring nsg</span></span>
* <span data-ttu-id="5bdad-1260">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1260">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5bdad-1261">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1261">Support managed service identities</span></span>
* <span data-ttu-id="5bdad-1262">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1262">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5bdad-1263">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1263">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5bdad-1264">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1264">May 10, 2017</span></span>

<span data-ttu-id="5bdad-1265">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5bdad-1265">Version 2.0.6</span></span>

* <span data-ttu-id="5bdad-1266">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="5bdad-1266">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5bdad-1267">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1267">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5bdad-1268">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="5bdad-1268">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5bdad-1269">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="5bdad-1269">Include Cognitive Services module</span></span>
* <span data-ttu-id="5bdad-1270">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="5bdad-1270">Include Service Fabric module</span></span>
* <span data-ttu-id="5bdad-1271">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="5bdad-1271">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5bdad-1272">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1272">Add support for CDN commands</span></span>
* <span data-ttu-id="5bdad-1273">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-1273">Remove Container module</span></span>
* <span data-ttu-id="5bdad-1274">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1274">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5bdad-1275">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1275">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5bdad-1276">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-1276">Core</span></span>

* <span data-ttu-id="5bdad-1277">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="5bdad-1277">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5bdad-1278">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1278">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5bdad-1279">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1279">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5bdad-1280">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1280">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5bdad-1281">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1281">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5bdad-1282">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1282">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5bdad-1283">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1283">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5bdad-1284">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1284">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5bdad-1285">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1285">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5bdad-1286">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="5bdad-1286">core: Improved performance</span></span>
* <span data-ttu-id="5bdad-1287">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1287">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5bdad-1288">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="5bdad-1288">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1289">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1289">ACS</span></span>

* <span data-ttu-id="5bdad-1290">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1290">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5bdad-1291">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="5bdad-1291">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5bdad-1292">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="5bdad-1292">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5bdad-1293">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1293">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-1294">AppService</span><span class="sxs-lookup"><span data-stu-id="5bdad-1294">AppService</span></span>

* <span data-ttu-id="5bdad-1295">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1295">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5bdad-1296">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1296">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5bdad-1297">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1297">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5bdad-1298">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="5bdad-1298">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5bdad-1299">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="5bdad-1299">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5bdad-1300">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1300">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5bdad-1301">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1301">support slot swap with preview</span></span>
* <span data-ttu-id="5bdad-1302">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1302">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5bdad-1303">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1303">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bdad-1304">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bdad-1304">CosmosDB</span></span>

* <span data-ttu-id="5bdad-1305">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="5bdad-1305">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5bdad-1306">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1306">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5bdad-1307">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1307">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5bdad-1308">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1308">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bdad-1309">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bdad-1309">Data Lake Analytics</span></span>

* <span data-ttu-id="5bdad-1310">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1310">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5bdad-1311">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1311">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5bdad-1312">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1312">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5bdad-1313">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="5bdad-1313">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5bdad-1314">테이블</span><span class="sxs-lookup"><span data-stu-id="5bdad-1314">Table</span></span>
  * <span data-ttu-id="5bdad-1315">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="5bdad-1315">Table valued function</span></span>
  * <span data-ttu-id="5bdad-1316">보기</span><span class="sxs-lookup"><span data-stu-id="5bdad-1316">View</span></span>
  * <span data-ttu-id="5bdad-1317">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1317">Table Statistics.</span></span> <span data-ttu-id="5bdad-1318">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1318">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bdad-1319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bdad-1319">Data Lake Store</span></span>

* <span data-ttu-id="5bdad-1320">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="5bdad-1320">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5bdad-1321">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1321">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5bdad-1322">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1322">missed help for access show.</span></span> <span data-ttu-id="5bdad-1323">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1323">adding it.</span></span> <span data-ttu-id="5bdad-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5bdad-1325">찾기</span><span class="sxs-lookup"><span data-stu-id="5bdad-1325">Find</span></span>

* <span data-ttu-id="5bdad-1326">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="5bdad-1326">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bdad-1327">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bdad-1327">KeyVault</span></span>

* <span data-ttu-id="5bdad-1328">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1328">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5bdad-1329">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1329">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5bdad-1330">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1330">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5bdad-1331">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1331">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5bdad-1332">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1332">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5bdad-1333">랩</span><span class="sxs-lookup"><span data-stu-id="5bdad-1333">Lab</span></span>

* <span data-ttu-id="5bdad-1334">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1334">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5bdad-1335">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1335">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5bdad-1336">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="5bdad-1336">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5bdad-1337">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="5bdad-1337">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5bdad-1338">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1338">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5bdad-1339">모니터</span><span class="sxs-lookup"><span data-stu-id="5bdad-1339">Monitor</span></span>

* <span data-ttu-id="5bdad-1340">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1340">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5bdad-1341">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1341">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5bdad-1342">네트워크</span><span class="sxs-lookup"><span data-stu-id="5bdad-1342">Network</span></span>

* <span data-ttu-id="5bdad-1343">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1343">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5bdad-1344">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1344">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5bdad-1345">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1345">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5bdad-1346">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1346">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5bdad-1347">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1347">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5bdad-1348">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1348">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5bdad-1349">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1349">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5bdad-1350">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1350">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5bdad-1351">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1351">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5bdad-1352">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1352">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5bdad-1353">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="5bdad-1353">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5bdad-1354">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1354">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5bdad-1355">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1355">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5bdad-1356">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1356">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5bdad-1357">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1357">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5bdad-1358">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1358">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5bdad-1359">프로필</span><span class="sxs-lookup"><span data-stu-id="5bdad-1359">Profile</span></span>

* <span data-ttu-id="5bdad-1360">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1360">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5bdad-1361">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1361">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5bdad-1362">Redis</span><span class="sxs-lookup"><span data-stu-id="5bdad-1362">Redis</span></span>

* <span data-ttu-id="5bdad-1363">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1363">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5bdad-1364">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="5bdad-1364">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5bdad-1365">리소스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1365">Resource</span></span>

* <span data-ttu-id="5bdad-1366">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1366">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5bdad-1367">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1367">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5bdad-1368">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1368">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5bdad-1369">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1369">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5bdad-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5bdad-1371">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1371">Add docs for az lock update.</span></span> <span data-ttu-id="5bdad-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5bdad-1373">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1373">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5bdad-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5bdad-1375">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1375">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5bdad-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5bdad-1377">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1377">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5bdad-1378">역할</span><span class="sxs-lookup"><span data-stu-id="5bdad-1378">Role</span></span>

* <span data-ttu-id="5bdad-1379">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1379">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5bdad-1380">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1380">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5bdad-1381">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1381">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5bdad-1382">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="5bdad-1382">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5bdad-1383">SQL</span><span class="sxs-lookup"><span data-stu-id="5bdad-1383">SQL</span></span>

* <span data-ttu-id="5bdad-1384">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="5bdad-1384">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5bdad-1385">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1385">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5bdad-1386">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-1386">Storage</span></span>

* <span data-ttu-id="5bdad-1387">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="5bdad-1387">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5bdad-1388">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1388">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5bdad-1389">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1389">Add support for large block blob upload</span></span>
* <span data-ttu-id="5bdad-1390">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="5bdad-1390">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-1391">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-1391">VM</span></span>

* <span data-ttu-id="5bdad-1392">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="5bdad-1392">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5bdad-1393">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1393">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5bdad-1394">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5bdad-1394">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5bdad-1395">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5bdad-1395">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5bdad-1396">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1396">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5bdad-1397">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="5bdad-1397">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5bdad-1398">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1398">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5bdad-1399">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1399">April 3, 2017</span></span>

<span data-ttu-id="5bdad-1400">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5bdad-1400">Version 2.0.2</span></span>

<span data-ttu-id="5bdad-1401">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1401">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5bdad-1402">코어</span><span class="sxs-lookup"><span data-stu-id="5bdad-1402">Core</span></span>

* <span data-ttu-id="5bdad-1403">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="5bdad-1403">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5bdad-1404">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1404">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5bdad-1405">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1405">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5bdad-1406">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1406">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5bdad-1407">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1407">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5bdad-1408">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1408">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5bdad-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5bdad-1410">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1410">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5bdad-1411">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="5bdad-1411">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5bdad-1412">ACS</span><span class="sxs-lookup"><span data-stu-id="5bdad-1412">ACS</span></span>

* <span data-ttu-id="5bdad-1413">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1413">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5bdad-1414">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1414">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5bdad-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5bdad-1416">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1416">Add support for windows clusters.</span></span> <span data-ttu-id="5bdad-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5bdad-1418">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1418">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5bdad-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5bdad-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="5bdad-1420">AppService</span></span>

* <span data-ttu-id="5bdad-1421">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1421">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5bdad-1422">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1422">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5bdad-1423">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1423">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5bdad-1424">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1424">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5bdad-1425">DataLake</span><span class="sxs-lookup"><span data-stu-id="5bdad-1425">DataLake</span></span>

* <span data-ttu-id="5bdad-1426">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1426">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5bdad-1427">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="5bdad-1427">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5bdad-1428">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="5bdad-1428">DocuemntDB</span></span>

* <span data-ttu-id="5bdad-1429">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1429">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5bdad-1430">VM</span><span class="sxs-lookup"><span data-stu-id="5bdad-1430">VM</span></span>

* <span data-ttu-id="5bdad-1431">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1431">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5bdad-1432">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1432">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5bdad-1433">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1433">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5bdad-1434">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1434">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5bdad-1435">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1435">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5bdad-1436">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1436">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="5bdad-1437">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="5bdad-1437">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5bdad-1438">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="5bdad-1438">February 27, 2017</span></span>

<span data-ttu-id="5bdad-1439">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5bdad-1439">Version 2.0.0</span></span>

<span data-ttu-id="5bdad-1440">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1440">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5bdad-1441">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1441">Container Service (acs)</span></span>
- <span data-ttu-id="5bdad-1442">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="5bdad-1442">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5bdad-1443">네트워킹</span><span class="sxs-lookup"><span data-stu-id="5bdad-1443">Networking</span></span>
- <span data-ttu-id="5bdad-1444">Storage</span><span class="sxs-lookup"><span data-stu-id="5bdad-1444">Storage</span></span>

<span data-ttu-id="5bdad-1445">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1445">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5bdad-1446">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1446">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5bdad-1447">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1447">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5bdad-1448">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1448">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5bdad-1449">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1449">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5bdad-1450">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5bdad-1450">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5bdad-1451">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="5bdad-1451">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5bdad-1452">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="5bdad-1452">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5bdad-1453">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="5bdad-1453">Provide feedback from the command line with the `az feedback` command</span></span>


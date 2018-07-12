---
title: Azure CLI 2.0 릴리스 정보
description: Azure CLI 2.0 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 102152b7d99de253ccb2fea09b99be91e3c9135e
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439672"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="b3904-103">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="b3904-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="b3904-104">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="b3904-104">July 3, 2018</span></span>

<span data-ttu-id="b3904-105">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="b3904-105">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="b3904-106">AKS</span><span class="sxs-lookup"><span data-stu-id="b3904-106">AKS</span></span>

* <span data-ttu-id="b3904-107">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-107">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="b3904-108">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="b3904-108">July 3, 2018</span></span>

<span data-ttu-id="b3904-109">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="b3904-109">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="b3904-110">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-110">Core</span></span>

* <span data-ttu-id="b3904-111">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-111">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-112">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-112">ACR</span></span>

* <span data-ttu-id="b3904-113">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-113">Added polling build status</span></span>
* <span data-ttu-id="b3904-114">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-114">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="b3904-115">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-115">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-116">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-116">ACS</span></span>

* <span data-ttu-id="b3904-117">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-117">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="b3904-118">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-118">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="b3904-119">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="b3904-119">Updated options for `aks browse` command.</span></span> <span data-ttu-id="b3904-120">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-120">Added `--listen-port` support</span></span>
* <span data-ttu-id="b3904-121">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="b3904-121">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="b3904-122">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="b3904-122">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="b3904-123">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-123">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-124">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-124">AppService</span></span>

* <span data-ttu-id="b3904-125">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-125">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="b3904-126">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-126">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="b3904-127">Backup</span><span class="sxs-lookup"><span data-stu-id="b3904-127">Backup</span></span>

* <span data-ttu-id="b3904-128">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-128">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="b3904-129">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b3904-129">BatchAI</span></span>

* <span data-ttu-id="b3904-130">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-130">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="b3904-131">클라우드</span><span class="sxs-lookup"><span data-stu-id="b3904-131">Cloud</span></span>

* <span data-ttu-id="b3904-132">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-132">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="b3904-133">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-133">Container</span></span>

* <span data-ttu-id="b3904-134">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-134">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="b3904-135">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-135">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="b3904-136">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-136">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-137">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-137">Extension</span></span>

* <span data-ttu-id="b3904-138">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-138">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="b3904-139">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-139">Network</span></span>

* <span data-ttu-id="b3904-140">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="b3904-140">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="b3904-141">Rdbms</span><span class="sxs-lookup"><span data-stu-id="b3904-141">Rdbms</span></span>

* <span data-ttu-id="b3904-142">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-142">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-143">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-143">Resource</span></span>

* <span data-ttu-id="b3904-144">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-144">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-145">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-145">VM</span></span>

* <span data-ttu-id="b3904-146">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-146">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="b3904-147">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="b3904-147">June 25, 2018</span></span>

<span data-ttu-id="b3904-148">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="b3904-148">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="b3904-149">CLI</span><span class="sxs-lookup"><span data-stu-id="b3904-149">CLI</span></span>

* <span data-ttu-id="b3904-150">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-150">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="b3904-151">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="b3904-151">June 19, 2018</span></span>

<span data-ttu-id="b3904-152">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="b3904-152">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="b3904-153">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-153">Core</span></span>

* <span data-ttu-id="b3904-154">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-154">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-155">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-155">ACR</span></span>

* <span data-ttu-id="b3904-156">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-156">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="b3904-157">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-157">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-158">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-158">ACS</span></span>

* <span data-ttu-id="b3904-159">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="b3904-159">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="b3904-160">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-160">Added `--update` support</span></span>
* <span data-ttu-id="b3904-161">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-161">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="b3904-162">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="b3904-162">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="b3904-163">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-163">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="b3904-164">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-164">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="b3904-165">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-165">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="b3904-166">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-166">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span> 

### <a name="appservice"></a><span data-ttu-id="b3904-167">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-167">AppService</span></span>

* <span data-ttu-id="b3904-168">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-168">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="b3904-169">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-169">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-170">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-170">Batch</span></span>

* <span data-ttu-id="b3904-171">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-171">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b3904-172">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b3904-172">Batch AI</span></span>

* <span data-ttu-id="b3904-173">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="b3904-173">Added support for workspaces.</span></span> <span data-ttu-id="b3904-174">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-174">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="b3904-175">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="b3904-175">Added support for experiments.</span></span> <span data-ttu-id="b3904-176">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-176">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="b3904-177">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-177">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="b3904-178">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="b3904-178">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="b3904-179">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-179">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="b3904-180">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-180">Added support for `--ids` to `batchai` commands</span></span> 
* <span data-ttu-id="b3904-181">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="b3904-181">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="b3904-182">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="b3904-182">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="b3904-183">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="b3904-183">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="b3904-184">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="b3904-184">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="b3904-185">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="b3904-185">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="b3904-186">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="b3904-186">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="b3904-187">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="b3904-187">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="b3904-188">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-188">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="b3904-189">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="b3904-189">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="b3904-190">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="b3904-190">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="b3904-191">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="b3904-191">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="b3904-192">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="b3904-192">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="b3904-193">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="b3904-193">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="b3904-194">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="b3904-194">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="b3904-195">지도</span><span class="sxs-lookup"><span data-stu-id="b3904-195">Maps</span></span>

* <span data-ttu-id="b3904-196">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-196">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="b3904-197">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-197">Network</span></span>

* <span data-ttu-id="b3904-198">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-198">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="b3904-199">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-199">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="b3904-200">#6502</span><span class="sxs-lookup"><span data-stu-id="b3904-200">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="b3904-201">예약</span><span class="sxs-lookup"><span data-stu-id="b3904-201">Reservations</span></span>

* <span data-ttu-id="b3904-202">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-202">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="b3904-203">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-203">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="b3904-204">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="b3904-204">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="b3904-205">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-205">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="b3904-206">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-206">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="b3904-207">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-207">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="b3904-208">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-208">Role</span></span>

* <span data-ttu-id="b3904-209">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="b3904-209">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-210">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-210">SQL</span></span>

* <span data-ttu-id="b3904-211">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-211">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-212">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-212">Storage</span></span>

* <span data-ttu-id="b3904-213">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="b3904-213">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-214">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-214">VM</span></span>

* <span data-ttu-id="b3904-215">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="b3904-215">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="b3904-216">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-216">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="b3904-217">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-217">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="b3904-218">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="b3904-218">June 13, 2018</span></span>

<span data-ttu-id="b3904-219">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="b3904-219">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="b3904-220">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-220">Core</span></span>

* <span data-ttu-id="b3904-221">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="b3904-221">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="b3904-222">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="b3904-222">June 13, 2018</span></span>

<span data-ttu-id="b3904-223">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="b3904-223">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="b3904-224">AKS</span><span class="sxs-lookup"><span data-stu-id="b3904-224">AKS</span></span>

* <span data-ttu-id="b3904-225">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-225">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="b3904-226">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="b3904-226">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="b3904-227">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-227">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="b3904-228">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-228">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="b3904-229">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-229">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-230">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-230">AppService</span></span>

* <span data-ttu-id="b3904-231">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-231">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="b3904-232">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="b3904-232">June 5, 2018</span></span>

<span data-ttu-id="b3904-233">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="b3904-233">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-234">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-234">Interactive</span></span>

* <span data-ttu-id="b3904-235">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="b3904-235">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="b3904-236">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="b3904-236">June 5, 2018</span></span>

<span data-ttu-id="b3904-237">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="b3904-237">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="b3904-238">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-238">Core</span></span>

* <span data-ttu-id="b3904-239">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-239">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="b3904-240">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-240">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-241">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-241">ACR</span></span>

* <span data-ttu-id="b3904-242">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-242">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="b3904-243">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-243">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="b3904-244">AKS</span><span class="sxs-lookup"><span data-stu-id="b3904-244">AKS</span></span>

* <span data-ttu-id="b3904-245">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-245">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-246">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-246">Batch</span></span>

* <span data-ttu-id="b3904-247">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="b3904-247">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-248">IOT</span><span class="sxs-lookup"><span data-stu-id="b3904-248">IOT</span></span>

* <span data-ttu-id="b3904-249">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-249">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="b3904-250">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-250">Network</span></span>

* <span data-ttu-id="b3904-251">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="b3904-251">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="b3904-252">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="b3904-252">Policy Insights</span></span>

* <span data-ttu-id="b3904-253">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-253">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="b3904-254">ARM</span><span class="sxs-lookup"><span data-stu-id="b3904-254">ARM</span></span>

* <span data-ttu-id="b3904-255">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-255">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-256">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-256">SQL</span></span>

* <span data-ttu-id="b3904-257">관리형 새 인스턴스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-257">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="b3904-258">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-258">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="b3904-259">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-259">Storage</span></span>

* <span data-ttu-id="b3904-260">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="b3904-260">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-261">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-261">VM</span></span>

* <span data-ttu-id="b3904-262">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-262">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="b3904-263">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-263">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="b3904-264">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-264">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="b3904-265">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="b3904-265">May 22, 2018</span></span>

<span data-ttu-id="b3904-266">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="b3904-266">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="b3904-267">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-267">Core</span></span>

* <span data-ttu-id="b3904-268">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-268">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-269">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-269">ACS</span></span>

* <span data-ttu-id="b3904-270">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-270">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="b3904-271">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-271">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-272">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-272">AppService</span></span>

* <span data-ttu-id="b3904-273">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-273">Improved generic update commands</span></span>
* <span data-ttu-id="b3904-274">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-274">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="b3904-275">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-275">Container</span></span>

* <span data-ttu-id="b3904-276">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-276">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="b3904-277">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-277">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-278">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-278">Extension</span></span>

* <span data-ttu-id="b3904-279">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-279">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-280">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-280">Interactive</span></span>

* <span data-ttu-id="b3904-281">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-281">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="b3904-282">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="b3904-282">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-283">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b3904-283">KeyVault</span></span>

* <span data-ttu-id="b3904-284">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="b3904-284">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="b3904-285">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-285">Network</span></span>

* <span data-ttu-id="b3904-286">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="b3904-286">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="b3904-287">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-287">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-288">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-288">SQL</span></span>

* <span data-ttu-id="b3904-289">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="b3904-289">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="b3904-290">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="b3904-290">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="b3904-291">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-291">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="b3904-292">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-292">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="b3904-293">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-293">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="b3904-294">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="b3904-294">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="b3904-295">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-295">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="b3904-296">`edition`</span><span class="sxs-lookup"><span data-stu-id="b3904-296">`edition`.</span></span> <span data-ttu-id="b3904-297">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-297">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="b3904-298">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="b3904-298">`elasticPoolName`.</span></span> <span data-ttu-id="b3904-299">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-299">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="b3904-300">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-300">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="b3904-301">`edition`</span><span class="sxs-lookup"><span data-stu-id="b3904-301">`edition`.</span></span> <span data-ttu-id="b3904-302">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="b3904-302">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="b3904-303">`dtu`</span><span class="sxs-lookup"><span data-stu-id="b3904-303">`dtu`.</span></span> <span data-ttu-id="b3904-304">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="b3904-304">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="b3904-305">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="b3904-305">`databaseDtuMin`.</span></span> <span data-ttu-id="b3904-306">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="b3904-306">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="b3904-307">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="b3904-307">`databaseDtuMax`.</span></span> <span data-ttu-id="b3904-308">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="b3904-308">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="b3904-309">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-309">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="b3904-310">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-310">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-311">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-311">Storage</span></span>

* <span data-ttu-id="b3904-312">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-312">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="b3904-313">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-313">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-314">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-314">VM</span></span>

* <span data-ttu-id="b3904-315">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="b3904-315">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="b3904-316">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="b3904-316">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="b3904-317">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="b3904-317">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="b3904-318">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="b3904-318">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="b3904-319">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-319">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="b3904-320">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="b3904-320">May 7, 2018</span></span>

<span data-ttu-id="b3904-321">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="b3904-321">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="b3904-322">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-322">Core</span></span>

* <span data-ttu-id="b3904-323">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-323">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="b3904-324">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-324">Added limited support for positional arguments</span></span>
* <span data-ttu-id="b3904-325">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-325">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="b3904-326">#5591</span><span class="sxs-lookup"><span data-stu-id="b3904-326">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="b3904-327">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-327">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="b3904-328">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-328">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="b3904-329">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-329">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="b3904-330">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-330">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="b3904-331">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-331">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-332">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-332">ACR</span></span>

* <span data-ttu-id="b3904-333">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-333">Added ACR Build commands</span></span>
* <span data-ttu-id="b3904-334">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-334">Improved resource not found error messages</span></span>
* <span data-ttu-id="b3904-335">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-335">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="b3904-336">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-336">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="b3904-337">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-337">Improved repository commands error messages</span></span>
* <span data-ttu-id="b3904-338">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-338">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-339">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-339">ACS</span></span>

* <span data-ttu-id="b3904-340">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-340">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="b3904-341">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-341">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="b3904-342">AMS</span><span class="sxs-lookup"><span data-stu-id="b3904-342">AMS</span></span>

* <span data-ttu-id="b3904-343">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="b3904-343">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-344">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-344">Appservice</span></span>

* <span data-ttu-id="b3904-345">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-345">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="b3904-346">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-346">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="b3904-347">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-347">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="b3904-348">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-348">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b3904-349">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b3904-349">Batch AI</span></span>

* <span data-ttu-id="b3904-350">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-350">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b3904-351">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b3904-351">Cognitive Services</span></span>

* <span data-ttu-id="b3904-352">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-352">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="b3904-353">Consumption</span><span class="sxs-lookup"><span data-stu-id="b3904-353">Consumption</span></span>

* <span data-ttu-id="b3904-354">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-354">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="b3904-355">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-355">Container</span></span>

* <span data-ttu-id="b3904-356">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-356">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="b3904-357">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b3904-357">Cosmos DB</span></span>

* <span data-ttu-id="b3904-358">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b3904-358">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="b3904-359">DMS</span><span class="sxs-lookup"><span data-stu-id="b3904-359">DMS</span></span>

* <span data-ttu-id="b3904-360">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-360">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-361">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-361">Extension</span></span>

* <span data-ttu-id="b3904-362">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-362">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-363">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-363">Interactive</span></span>

* <span data-ttu-id="b3904-364">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-364">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="b3904-365">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="b3904-365">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="b3904-366">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-366">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="b3904-367">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-367">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="b3904-368">랩</span><span class="sxs-lookup"><span data-stu-id="b3904-368">Lab</span></span>

* <span data-ttu-id="b3904-369">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-369">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="b3904-370">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-370">Network</span></span>

* <span data-ttu-id="b3904-371">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-371">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="b3904-372">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-372">Profile</span></span>

* <span data-ttu-id="b3904-373">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-373">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="b3904-374">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-374">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="b3904-375">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-375">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="b3904-376">Redis</span><span class="sxs-lookup"><span data-stu-id="b3904-376">Redis</span></span>

* <span data-ttu-id="b3904-377">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-377">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="b3904-378">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-378">Deprecated `redis list-all`.</span></span> <span data-ttu-id="b3904-379">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="b3904-379">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="b3904-380">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-380">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="b3904-381">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-381">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="b3904-382">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-382">Role</span></span>

* <span data-ttu-id="b3904-383">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-383">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-384">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-384">Storage</span></span>

* <span data-ttu-id="b3904-385">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-385">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="b3904-386">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="b3904-386">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="b3904-387">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="b3904-387">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="b3904-388">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-388">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="b3904-389">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-389">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-390">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-390">VM</span></span>

* <span data-ttu-id="b3904-391">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-391">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="b3904-392">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-392">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="b3904-393">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="b3904-393">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="b3904-394">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-394">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="b3904-395">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-395">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="b3904-396">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-396">Added write accelerator support</span></span> 
* <span data-ttu-id="b3904-397">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-397">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="b3904-398">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-398">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="b3904-399">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-399">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="b3904-400">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="b3904-400">April 10, 2018</span></span>

<span data-ttu-id="b3904-401">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="b3904-401">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-402">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-402">ACR</span></span>

* <span data-ttu-id="b3904-403">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="b3904-403">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-404">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-404">ACS</span></span>

* <span data-ttu-id="b3904-405">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-405">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-406">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-406">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="b3904-408">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-408">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="b3904-409">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b3904-409">BatchAI</span></span>

* <span data-ttu-id="b3904-410">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-410">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="b3904-411">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="b3904-411">Job level mounting</span></span>
 - <span data-ttu-id="b3904-412">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="b3904-412">Environment variables with secret values</span></span>
 - <span data-ttu-id="b3904-413">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-413">Performance counters settings</span></span>
 - <span data-ttu-id="b3904-414">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="b3904-414">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="b3904-415">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-415">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="b3904-416">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="b3904-416">Usage and limits reporting</span></span>
 - <span data-ttu-id="b3904-417">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-417">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="b3904-418">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-418">Support for custom images</span></span>
 - <span data-ttu-id="b3904-419">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-419">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="b3904-420">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-420">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="b3904-421">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-421">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="b3904-422">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-422">National clouds are supported</span></span>
* <span data-ttu-id="b3904-423">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-423">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="b3904-424">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="b3904-424">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="b3904-425">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-425">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="b3904-426">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-426">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="b3904-427">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="b3904-427">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="b3904-428">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="b3904-428">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="b3904-429">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-429">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="b3904-430">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-430">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="b3904-431">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-431">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="b3904-432">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-432">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="b3904-433">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-433">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="b3904-434">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="b3904-434">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="b3904-435">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-435">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="b3904-436">결제</span><span class="sxs-lookup"><span data-stu-id="b3904-436">Billing</span></span>

* <span data-ttu-id="b3904-437">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-437">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="b3904-438">Consumption</span><span class="sxs-lookup"><span data-stu-id="b3904-438">Consumption</span></span>

* <span data-ttu-id="b3904-439">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-439">Added `marketplace` commands</span></span>
* <span data-ttu-id="b3904-440">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-440">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="b3904-441">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-441">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="b3904-442">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-442">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="b3904-443">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-443">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="b3904-444">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-444">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="b3904-445">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-445">Container</span></span>

* <span data-ttu-id="b3904-446">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="b3904-446">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="b3904-447">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="b3904-447">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-448">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-448">Extension</span></span>

* <span data-ttu-id="b3904-449">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-449">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-450">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-450">Interactive</span></span>

* <span data-ttu-id="b3904-451">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-451">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="b3904-452">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-452">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="b3904-453">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-453">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="b3904-454">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-454">Network</span></span>

* <span data-ttu-id="b3904-455">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-455">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="b3904-456">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-456">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="b3904-457">#4910</span><span class="sxs-lookup"><span data-stu-id="b3904-457">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="b3904-458">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-458">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="b3904-459">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="b3904-459">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="b3904-460">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-460">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="b3904-461">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-461">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="b3904-462">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-462">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-463">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-463">Profile</span></span>

* <span data-ttu-id="b3904-464">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-464">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="b3904-465">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-465">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="b3904-466">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b3904-466">RDBMS</span></span>

* <span data-ttu-id="b3904-467">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-467">Added `georestore` command</span></span>
* <span data-ttu-id="b3904-468">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-468">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-469">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-469">Resource</span></span>

* <span data-ttu-id="b3904-470">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-470">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="b3904-471">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-471">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-472">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-472">SQL</span></span>

* <span data-ttu-id="b3904-473">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-473">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-474">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-474">Storage</span></span>

* <span data-ttu-id="b3904-475">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-475">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-476">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-476">VM</span></span>

* <span data-ttu-id="b3904-477">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-477">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="b3904-478">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-478">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="b3904-480">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-480">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="b3904-481">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-481">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="b3904-482">#5718</span><span class="sxs-lookup"><span data-stu-id="b3904-482">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="b3904-483">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-483">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="b3904-484">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="b3904-484">March 27, 2018</span></span>

<span data-ttu-id="b3904-485">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="b3904-485">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="b3904-486">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-486">Core</span></span>

* <span data-ttu-id="b3904-487">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="b3904-487">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-488">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-488">ACS</span></span>

* <span data-ttu-id="b3904-489">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-489">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-490">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-490">Appservice</span></span>

* <span data-ttu-id="b3904-491">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-491">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="b3904-492">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-492">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="b3904-493">Backup</span><span class="sxs-lookup"><span data-stu-id="b3904-493">Backup</span></span>

* <span data-ttu-id="b3904-494">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-494">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="b3904-495">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-495">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="b3904-496">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-496">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="b3904-497">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-497">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="b3904-498">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-498">Container</span></span>

* <span data-ttu-id="b3904-499">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-499">Added `container exec` command.</span></span> <span data-ttu-id="b3904-500">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-500">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="b3904-501">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-501">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-502">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-502">Extension</span></span>

* <span data-ttu-id="b3904-503">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-503">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="b3904-504">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-504">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="b3904-505">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-505">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-506">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-506">Interactive</span></span>

* <span data-ttu-id="b3904-507">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="b3904-507">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="b3904-508">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-508">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="b3904-509">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="b3904-509">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="b3904-510">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-510">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="b3904-511">랩</span><span class="sxs-lookup"><span data-stu-id="b3904-511">Lab</span></span>

* <span data-ttu-id="b3904-512">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-512">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-513">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-513">Monitor</span></span>

* <span data-ttu-id="b3904-514">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-514">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="b3904-515">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="b3904-515">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="b3904-516">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-516">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="b3904-517">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-517">Network</span></span>

* <span data-ttu-id="b3904-518">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-518">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-519">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-519">Profile</span></span>

* <span data-ttu-id="b3904-520">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-520">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="b3904-521">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b3904-521">RDBMS</span></span>

* <span data-ttu-id="b3904-522">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-522">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-523">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-523">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="b3904-525">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-525">Role</span></span>

* <span data-ttu-id="b3904-526">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-526">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="b3904-527">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-527">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="b3904-528">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-528">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="b3904-529">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-529">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="b3904-530">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-530">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-531">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-531">Storage</span></span>

* <span data-ttu-id="b3904-532">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-532">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="b3904-533">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="b3904-533">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-534">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-534">VM</span></span>

* <span data-ttu-id="b3904-535">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-535">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="b3904-536">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-536">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="b3904-537">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-537">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="b3904-538">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-538">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="b3904-539">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="b3904-539">March 13, 2018</span></span>

<span data-ttu-id="b3904-540">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="b3904-540">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-541">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-541">ACR</span></span>

* <span data-ttu-id="b3904-542">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-542">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="b3904-543">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-543">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="b3904-544">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-544">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-545">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-545">ACS</span></span>

* <span data-ttu-id="b3904-546">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-546">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="b3904-547">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-547">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="b3904-548">Advisor</span><span class="sxs-lookup"><span data-stu-id="b3904-548">Advisor</span></span>

* <span data-ttu-id="b3904-549">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-549">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="b3904-550">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-550">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="b3904-551">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-551">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="b3904-552">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-552">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="b3904-553">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-553">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-554">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-554">Appservice</span></span>

* <span data-ttu-id="b3904-555">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-555">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="b3904-556">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-556">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="b3904-557">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="b3904-557">Eventhubs</span></span>

* <span data-ttu-id="b3904-558">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-558">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-559">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-559">Extension</span></span>

* <span data-ttu-id="b3904-560">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-560">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-561">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-561">Interactive</span></span>

* <span data-ttu-id="b3904-562">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="b3904-562">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="b3904-563">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="b3904-563">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="b3904-564">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-564">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="b3904-565">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-565">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-566">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-566">Monitor</span></span>

* <span data-ttu-id="b3904-567">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-567">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="b3904-568">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-568">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="b3904-569">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-569">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="b3904-570">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-570">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="b3904-571">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-571">Network</span></span>

* <span data-ttu-id="b3904-572">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-572">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="b3904-573">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="b3904-573">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="b3904-574">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-574">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="b3904-575">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-575">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-576">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-576">Profile</span></span>

* <span data-ttu-id="b3904-577">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-577">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="b3904-578">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-578">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="b3904-579">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b3904-579">RDBMS</span></span>

* <span data-ttu-id="b3904-580">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-580">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="b3904-581">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b3904-581">Service Bus</span></span>

* <span data-ttu-id="b3904-582">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-582">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-583">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-583">Storage</span></span>

* <span data-ttu-id="b3904-584">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-584">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="b3904-585">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-585">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-586">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-586">VM</span></span>

* <span data-ttu-id="b3904-587">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-587">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="b3904-588">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-588">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="b3904-589">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-589">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="b3904-590">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-590">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="b3904-591">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="b3904-591">February 27, 2018</span></span>

<span data-ttu-id="b3904-592">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="b3904-592">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="b3904-593">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-593">Core</span></span>

* <span data-ttu-id="b3904-594">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-594">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="b3904-595">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-595">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="b3904-596">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-596">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-597">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-597">ACS</span></span>

* <span data-ttu-id="b3904-598">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-598">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="b3904-599">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-599">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="b3904-600">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-600">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="b3904-601">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-601">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-602">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-602">Appservice</span></span>

* <span data-ttu-id="b3904-603">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="b3904-603">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="b3904-604">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-604">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b3904-605">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b3904-605">Cognitive Services</span></span>

* <span data-ttu-id="b3904-606">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-606">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="b3904-607">Consumption</span><span class="sxs-lookup"><span data-stu-id="b3904-607">Consumption</span></span>

* <span data-ttu-id="b3904-608">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-608">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="b3904-609">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-609">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="b3904-610">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-610">Container</span></span>

* <span data-ttu-id="b3904-611">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-611">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="b3904-612">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-612">Network</span></span>

* <span data-ttu-id="b3904-613">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-613">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-614">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-614">Resource</span></span>

* <span data-ttu-id="b3904-615">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-615">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="b3904-616">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-616">Role</span></span>

* <span data-ttu-id="b3904-617">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-617">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-618">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-618">SQL</span></span>

* <span data-ttu-id="b3904-619">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-619">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-620">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-620">Storage</span></span>

* <span data-ttu-id="b3904-621">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="b3904-621">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-622">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-622">VM</span></span>

* <span data-ttu-id="b3904-623">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-623">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="b3904-624">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="b3904-624">February 13, 2018</span></span>

<span data-ttu-id="b3904-625">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="b3904-625">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="b3904-626">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-626">Core</span></span>

* <span data-ttu-id="b3904-627">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-627">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-628">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-628">ACS</span></span>

* <span data-ttu-id="b3904-629">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-629">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="b3904-630">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-630">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="b3904-631">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-631">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="b3904-632">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="b3904-632">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="b3904-633">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-633">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="b3904-634">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="b3904-634">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="b3904-635">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-635">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="b3904-636">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-636">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-637">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-637">Appservice</span></span>

* <span data-ttu-id="b3904-638">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-638">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="b3904-639">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-639">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="b3904-640">CDN</span><span class="sxs-lookup"><span data-stu-id="b3904-640">CDN</span></span>

* <span data-ttu-id="b3904-641">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-641">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="b3904-642">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-642">Container</span></span>

* <span data-ttu-id="b3904-643">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-643">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="b3904-644">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-644">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b3904-645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b3904-645">CosmosDB</span></span>

* <span data-ttu-id="b3904-646">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-646">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-647">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-647">Extension</span></span>

* <span data-ttu-id="b3904-648">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-648">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="b3904-649">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-649">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="b3904-650">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="b3904-650">Feedback</span></span>

* <span data-ttu-id="b3904-651">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-651">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-652">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-652">Interactive</span></span>

* <span data-ttu-id="b3904-653">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-653">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="b3904-654">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-654">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-655">IoT</span><span class="sxs-lookup"><span data-stu-id="b3904-655">IoT</span></span>

* <span data-ttu-id="b3904-656">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-656">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="b3904-657">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-657">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="b3904-658">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-658">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="b3904-659">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-659">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-660">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-660">Monitor</span></span>

* <span data-ttu-id="b3904-661">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-661">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="b3904-662">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-662">Network</span></span>

* <span data-ttu-id="b3904-663">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-663">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="b3904-664">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-664">Profile</span></span>

* <span data-ttu-id="b3904-665">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-665">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-666">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-666">Resource</span></span>

* <span data-ttu-id="b3904-667">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-667">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="b3904-668">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-668">Role</span></span>

* <span data-ttu-id="b3904-669">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-669">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-670">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-670">SQL</span></span>

* <span data-ttu-id="b3904-671">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-671">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="b3904-672">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-672">Added `sql db rename`</span></span>
* <span data-ttu-id="b3904-673">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-673">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-674">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-674">Storage</span></span>

* <span data-ttu-id="b3904-675">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-675">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-676">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-676">VM</span></span>

* <span data-ttu-id="b3904-677">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-677">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="b3904-678">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-678">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="b3904-679">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="b3904-679">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="b3904-680">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="b3904-680">January 31, 2018</span></span>

<span data-ttu-id="b3904-681">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="b3904-681">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="b3904-682">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-682">Core</span></span>

* <span data-ttu-id="b3904-683">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-683">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="b3904-684">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-684">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="b3904-685">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-685">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="b3904-686">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="b3904-686">Use `--verbose` to see</span></span>
* <span data-ttu-id="b3904-687">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-687">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-688">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-688">ACS</span></span>

* <span data-ttu-id="b3904-689">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-689">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="b3904-690">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="b3904-690">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-691">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-691">Appservice</span></span>

* <span data-ttu-id="b3904-692">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="b3904-692">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="b3904-693">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-693">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="b3904-694">CDN</span><span class="sxs-lookup"><span data-stu-id="b3904-694">CDN</span></span>

* <span data-ttu-id="b3904-695">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-695">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b3904-696">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b3904-696">CosmosDB</span></span>

* <span data-ttu-id="b3904-697">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-697">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-698">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-698">Interactive</span></span>

* <span data-ttu-id="b3904-699">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-699">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="b3904-700">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-700">Network</span></span>

* <span data-ttu-id="b3904-701">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-701">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="b3904-702">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-702">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="b3904-703">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-703">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="b3904-704">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-704">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="b3904-705">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-705">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="b3904-706">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="b3904-706">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="b3904-707">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-707">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="b3904-708">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-708">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="b3904-709">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-709">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="b3904-710">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="b3904-710">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-711">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-711">Profile</span></span>

* <span data-ttu-id="b3904-712">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-712">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-713">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-713">Resource</span></span>

* <span data-ttu-id="b3904-714">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-714">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-715">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-715">Storage</span></span>

* <span data-ttu-id="b3904-716">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-716">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="b3904-717">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-717">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="b3904-718">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-718">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="b3904-719">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-719">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="b3904-720">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-720">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-721">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-721">VM</span></span>

* <span data-ttu-id="b3904-722">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-722">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="b3904-723">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-723">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="b3904-724">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-724">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="b3904-725">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-725">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="b3904-726">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="b3904-726">January 17, 2018</span></span>

<span data-ttu-id="b3904-727">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="b3904-727">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-728">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-728">ACR</span></span>

* <span data-ttu-id="b3904-729">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-729">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="b3904-730">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-730">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-731">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-731">ACS</span></span>

* <span data-ttu-id="b3904-732">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-732">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="b3904-733">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-733">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-734">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-734">Appservice</span></span>

* <span data-ttu-id="b3904-735">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-735">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="b3904-736">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-736">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="b3904-737">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-737">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="b3904-738">Backup</span><span class="sxs-lookup"><span data-stu-id="b3904-738">Backup</span></span>

* <span data-ttu-id="b3904-739">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-739">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="b3904-740">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-740">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="b3904-741">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-741">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="b3904-742">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-742">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="b3904-743">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-743">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-744">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-744">Batch</span></span>

* <span data-ttu-id="b3904-745">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-745">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="b3904-746">클라우드</span><span class="sxs-lookup"><span data-stu-id="b3904-746">Cloud</span></span>

* <span data-ttu-id="b3904-747">클라우드에서 `--profile`을 설정할 때 끝점을 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-747">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="b3904-748">Consumption</span><span class="sxs-lookup"><span data-stu-id="b3904-748">Consumption</span></span>

* <span data-ttu-id="b3904-749">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-749">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="b3904-750">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b3904-750">Event Grid</span></span>

* <span data-ttu-id="b3904-751">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="b3904-751">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b3904-752">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="b3904-752">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b3904-753">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-753">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="b3904-754">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="b3904-754">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="b3904-755">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-755">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="b3904-756">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-756">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="b3904-757">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-757">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="b3904-758">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-758">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-759">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-759">Interactive</span></span>

* <span data-ttu-id="b3904-760">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-760">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="b3904-761">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-761">Fixed errors on startup</span></span>
* <span data-ttu-id="b3904-762">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-762">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-763">IoT</span><span class="sxs-lookup"><span data-stu-id="b3904-763">IoT</span></span>

* <span data-ttu-id="b3904-764">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-764">Added support for device provisioning service</span></span>
* <span data-ttu-id="b3904-765">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-765">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="b3904-766">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-766">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-767">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-767">Monitor</span></span>

* <span data-ttu-id="b3904-768">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-768">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="b3904-769">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="b3904-769">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="b3904-770">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-770">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="b3904-771">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-771">Network</span></span>

* <span data-ttu-id="b3904-772">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-772">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="b3904-773">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-773">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-774">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-774">Profile</span></span>

* <span data-ttu-id="b3904-775">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-775">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="b3904-776">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-776">Role</span></span>

* <span data-ttu-id="b3904-777">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-777">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b3904-778">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b3904-778">Service Fabric</span></span>

* <span data-ttu-id="b3904-779">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-779">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="b3904-780">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-780">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-781">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-781">VM</span></span>

* <span data-ttu-id="b3904-782">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-782">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="b3904-783">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-783">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="b3904-784">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-784">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="b3904-785">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-785">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="b3904-786">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-786">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="b3904-787">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-787">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="b3904-788">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-788">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="b3904-789">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-789">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="b3904-790">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="b3904-790">December 19, 2017</span></span>

<span data-ttu-id="b3904-791">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="b3904-791">Version 2.0.23</span></span>

* <span data-ttu-id="b3904-792">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-792">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="b3904-793">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-793">Container</span></span>

* <span data-ttu-id="b3904-794">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-794">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="b3904-795">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-795">Network</span></span>

* <span data-ttu-id="b3904-796">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-796">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="b3904-797">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-797">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-798">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-798">Storage</span></span>

* <span data-ttu-id="b3904-799">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-799">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-800">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-800">VM</span></span>

* <span data-ttu-id="b3904-801">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-801">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="b3904-802">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="b3904-802">December 5, 2017</span></span>

<span data-ttu-id="b3904-803">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="b3904-803">Version 2.0.22</span></span>

* <span data-ttu-id="b3904-804">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-804">Removed `az component` commands.</span></span> <span data-ttu-id="b3904-805">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="b3904-805">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="b3904-806">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-806">Core</span></span>
* <span data-ttu-id="b3904-807">`AZURE_US_GOV_CLOUD` AAD 권한 끝점이 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-807">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="b3904-808">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-808">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-809">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-809">ACS</span></span>

* <span data-ttu-id="b3904-810">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-810">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="b3904-811">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-811">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="b3904-812">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-812">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="b3904-813">Advisor</span><span class="sxs-lookup"><span data-stu-id="b3904-813">Advisor</span></span>

* <span data-ttu-id="b3904-814">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-814">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-815">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-815">Appservice</span></span>

* <span data-ttu-id="b3904-816">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-816">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="b3904-817">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-817">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="b3904-818">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-818">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="b3904-819">Consumption</span><span class="sxs-lookup"><span data-stu-id="b3904-819">Consumption</span></span>

* <span data-ttu-id="b3904-820">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-820">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="b3904-821">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-821">Container</span></span>

* <span data-ttu-id="b3904-822">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-822">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-823">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-823">Monitor</span></span>

* <span data-ttu-id="b3904-824">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-824">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-825">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-825">Resource</span></span>

* <span data-ttu-id="b3904-826">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-826">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="b3904-827">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-827">Role</span></span>

* <span data-ttu-id="b3904-828">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-828">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="b3904-829">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-829">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="b3904-830">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="b3904-830">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-831">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-831">SQL</span></span>

* <span data-ttu-id="b3904-832">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-832">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="b3904-833">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-833">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-834">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-834">VM</span></span>

* <span data-ttu-id="b3904-835">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-835">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="b3904-836">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="b3904-836">November 14, 2017</span></span>

<span data-ttu-id="b3904-837">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="b3904-837">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-838">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-838">ACR</span></span>

* <span data-ttu-id="b3904-839">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-839">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="b3904-840">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-840">ACS</span></span>

* <span data-ttu-id="b3904-841">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-841">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="b3904-842">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="b3904-842">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="b3904-843">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-843">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="b3904-844">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-844">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="b3904-845">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-845">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-846">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-846">Appservice</span></span>

* <span data-ttu-id="b3904-847">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-847">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="b3904-848">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-848">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="b3904-849">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-849">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="b3904-850">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-850">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="b3904-851">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-851">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="b3904-852">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="b3904-852">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-853">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-853">Batch</span></span>

* <span data-ttu-id="b3904-854">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-854">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="b3904-855">Batchai</span><span class="sxs-lookup"><span data-stu-id="b3904-855">Batchai</span></span>

* <span data-ttu-id="b3904-856">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-856">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="b3904-857">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-857">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="b3904-858">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-858">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="b3904-859">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-859">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="b3904-860">클라우드</span><span class="sxs-lookup"><span data-stu-id="b3904-860">Cloud</span></span>

* <span data-ttu-id="b3904-861">필요한 끝점이 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-861">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="b3904-862">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-862">Container</span></span>

* <span data-ttu-id="b3904-863">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-863">Added support to open multiple ports</span></span>
* <span data-ttu-id="b3904-864">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-864">Added container group restart policy</span></span>
* <span data-ttu-id="b3904-865">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-865">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="b3904-866">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="b3904-866">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b3904-867">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b3904-867">Data Lake Analytics</span></span>

* <span data-ttu-id="b3904-868">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-868">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b3904-869">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b3904-869">Data Lake Store</span></span>

* <span data-ttu-id="b3904-870">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-870">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-871">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-871">Extension</span></span>

* <span data-ttu-id="b3904-872">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-872">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="b3904-873">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-873">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-874">IoT</span><span class="sxs-lookup"><span data-stu-id="b3904-874">IoT</span></span>

* <span data-ttu-id="b3904-875">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-875">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-876">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-876">Monitor</span></span>

* <span data-ttu-id="b3904-877">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-877">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="b3904-878">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-878">Network</span></span>

* <span data-ttu-id="b3904-879">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-879">Added support for CAA DNS records</span></span>
* <span data-ttu-id="b3904-880">`traffic-manager profile update`로 끝점을 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-880">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="b3904-881">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-881">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="b3904-882">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-882">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="b3904-883">예약</span><span class="sxs-lookup"><span data-stu-id="b3904-883">Reservations</span></span>

* <span data-ttu-id="b3904-884">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-884">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-885">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-885">Resource</span></span>

* <span data-ttu-id="b3904-886">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-886">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-887">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-887">SQL</span></span>

* <span data-ttu-id="b3904-888">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-888">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-889">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-889">Storage</span></span>

* <span data-ttu-id="b3904-890">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-890">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="b3904-891">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-891">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="b3904-892">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-892">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="b3904-893">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="b3904-893">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="b3904-894">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-894">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="b3904-895">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-895">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="b3904-896">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-896">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-897">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-897">VM</span></span>

* <span data-ttu-id="b3904-898">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-898">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="b3904-899">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-899">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="b3904-900">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-900">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="b3904-901">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-901">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="b3904-902">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-902">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="b3904-903">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="b3904-903">October 24, 2017</span></span>

<span data-ttu-id="b3904-904">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="b3904-904">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="b3904-905">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-905">Core</span></span>

* <span data-ttu-id="b3904-906">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="b3904-906">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-907">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-907">ACR</span></span>

* <span data-ttu-id="b3904-908">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="b3904-908">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="b3904-909">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-909">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="b3904-910">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="b3904-910">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-911">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-911">ACS</span></span>

* <span data-ttu-id="b3904-912">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-912">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="b3904-913">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-913">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-914">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-914">Appservice</span></span>

* <span data-ttu-id="b3904-915">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-915">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="b3904-916">구성 요소</span><span class="sxs-lookup"><span data-stu-id="b3904-916">Component</span></span>

* <span data-ttu-id="b3904-917">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-917">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-918">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-918">Monitor</span></span>

* <span data-ttu-id="b3904-919">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-919">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-920">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-920">Resource</span></span>

* <span data-ttu-id="b3904-921">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-921">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="b3904-922">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-922">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-923">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-923">VM</span></span>

* <span data-ttu-id="b3904-924">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-924">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="b3904-925">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="b3904-925">October 9, 2017</span></span>

<span data-ttu-id="b3904-926">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="b3904-926">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="b3904-927">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-927">Core</span></span>

* <span data-ttu-id="b3904-928">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-928">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-929">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-929">Appservice</span></span>

* <span data-ttu-id="b3904-930">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-930">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-931">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-931">Batch</span></span>

* <span data-ttu-id="b3904-932">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-932">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="b3904-933">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-933">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="b3904-934">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-934">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="b3904-935">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-935">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="b3904-936">Batchai</span><span class="sxs-lookup"><span data-stu-id="b3904-936">Batchai</span></span>

* <span data-ttu-id="b3904-937">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-937">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-938">Keyvault</span><span class="sxs-lookup"><span data-stu-id="b3904-938">Keyvault</span></span>

* <span data-ttu-id="b3904-939">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-939">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="b3904-940">(#4448)</span><span class="sxs-lookup"><span data-stu-id="b3904-940">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="b3904-941">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-941">Network</span></span>

* <span data-ttu-id="b3904-942">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-942">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="b3904-943">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-943">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-944">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-944">Resource</span></span>

* <span data-ttu-id="b3904-945">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-945">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="b3904-946">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-946">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="b3904-947">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-947">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="b3904-948">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-948">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-949">Sql</span><span class="sxs-lookup"><span data-stu-id="b3904-949">Sql</span></span>

* <span data-ttu-id="b3904-950">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-950">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="b3904-951">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-951">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="b3904-952">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-952">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-953">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-953">Storage</span></span>

* <span data-ttu-id="b3904-954">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-954">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-955">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-955">Vm</span></span>

* <span data-ttu-id="b3904-956">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-956">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="b3904-957">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-957">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="b3904-958">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-958">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="b3904-959">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-959">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="b3904-960">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-960">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="b3904-961">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="b3904-961">September 22, 2017</span></span>

<span data-ttu-id="b3904-962">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="b3904-962">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-963">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-963">Resource</span></span>

* <span data-ttu-id="b3904-964">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-964">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="b3904-965">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-965">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="b3904-966">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-966">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="b3904-967">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-967">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="b3904-968">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-968">Network</span></span>

* <span data-ttu-id="b3904-969">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-969">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="b3904-970">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-970">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="b3904-971">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-971">Added `asg` application security group commands</span></span>
* <span data-ttu-id="b3904-972">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-972">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="b3904-973">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-973">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b3904-974">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-974">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="b3904-975">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-975">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-976">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-976">Storage</span></span>

* <span data-ttu-id="b3904-977">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-977">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b3904-978">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b3904-978">Eventgrid</span></span>

* <span data-ttu-id="b3904-979">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="b3904-979">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-980">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-980">SQL</span></span>

* <span data-ttu-id="b3904-981">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-981">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="b3904-982">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="b3904-982">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="b3904-983">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-983">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-984">Keyvault</span><span class="sxs-lookup"><span data-stu-id="b3904-984">Keyvault</span></span>

* <span data-ttu-id="b3904-985">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-985">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-986">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-986">VM</span></span>

* <span data-ttu-id="b3904-987">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-987">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="b3904-988">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="b3904-988">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="b3904-989">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-989">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="b3904-990">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-990">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="b3904-991">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-991">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="b3904-992">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-992">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-993">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-993">ACS</span></span>

* <span data-ttu-id="b3904-994">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-994">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-995">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-995">Appservice</span></span>

* <span data-ttu-id="b3904-996">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-996">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="b3904-997">Backup</span><span class="sxs-lookup"><span data-stu-id="b3904-997">Backup</span></span>

* <span data-ttu-id="b3904-998">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-998">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="b3904-999">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="b3904-999">September 11, 2017</span></span>

<span data-ttu-id="b3904-1000">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="b3904-1000">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="b3904-1001">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-1001">Core</span></span>

* <span data-ttu-id="b3904-1002">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1002">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="b3904-1003">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1003">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1004">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1004">Acs</span></span>

* <span data-ttu-id="b3904-1005">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1005">Added `acs list-locations` command</span></span>
* <span data-ttu-id="b3904-1006">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="b3904-1006">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1007">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-1007">Appservice</span></span>

* <span data-ttu-id="b3904-1008">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1008">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="b3904-1009">CDN</span><span class="sxs-lookup"><span data-stu-id="b3904-1009">CDN</span></span>

* <span data-ttu-id="b3904-1010">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1010">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="b3904-1011">내선 번호</span><span class="sxs-lookup"><span data-stu-id="b3904-1011">Extension</span></span>

* <span data-ttu-id="b3904-1012">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-1012">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-1013">Keyvault</span><span class="sxs-lookup"><span data-stu-id="b3904-1013">Keyvault</span></span>

* <span data-ttu-id="b3904-1014">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1014">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="b3904-1015">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-1015">Network</span></span>

* <span data-ttu-id="b3904-1016">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1016">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b3904-1017">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-1017">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="b3904-1018">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1018">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="b3904-1019">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1019">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b3904-1020">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1020">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-1021">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-1021">Resource</span></span>

* <span data-ttu-id="b3904-1022">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-1022">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="b3904-1023">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-1023">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="b3904-1024">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-1024">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="b3904-1025">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="b3904-1025">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-1026">SQL</span></span>

* <span data-ttu-id="b3904-1027">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1027">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1028">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1028">VM</span></span>

* <span data-ttu-id="b3904-1029">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1029">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="b3904-1030">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="b3904-1030">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="b3904-1031">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1031">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="b3904-1032">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1032">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="b3904-1033">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1033">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="b3904-1034">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="b3904-1034">August 31, 2017</span></span>

<span data-ttu-id="b3904-1035">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="b3904-1035">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-1036">Keyvault</span><span class="sxs-lookup"><span data-stu-id="b3904-1036">Keyvault</span></span>

* <span data-ttu-id="b3904-1037">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1037">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="b3904-1038">Sf</span><span class="sxs-lookup"><span data-stu-id="b3904-1038">Sf</span></span>

* <span data-ttu-id="b3904-1039">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1039">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-1040">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1040">Storage</span></span>

* <span data-ttu-id="b3904-1041">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1041">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="b3904-1042">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="b3904-1042">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="b3904-1043">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="b3904-1043">August 28, 2017</span></span>

<span data-ttu-id="b3904-1044">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="b3904-1044">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="b3904-1045">CLI</span><span class="sxs-lookup"><span data-stu-id="b3904-1045">CLI</span></span>

* <span data-ttu-id="b3904-1046">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1046">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1047">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1047">ACS</span></span>

* <span data-ttu-id="b3904-1048">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1048">Corrected preview regions</span></span>
* <span data-ttu-id="b3904-1049">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1049">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="b3904-1050">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1050">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1051">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-1051">Appservice</span></span>

* <span data-ttu-id="b3904-1052">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1052">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="b3904-1053">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1053">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="b3904-1054">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1054">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="b3904-1055">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1055">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="b3904-1056">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1056">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-1057">IoT</span><span class="sxs-lookup"><span data-stu-id="b3904-1057">IoT</span></span>

* <span data-ttu-id="b3904-1058">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1058">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="b3904-1059">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-1059">Network</span></span>

* <span data-ttu-id="b3904-1060">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1060">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b3904-1061">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1061">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="b3904-1062">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1062">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b3904-1063">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1063">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b3904-1064">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1064">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-1065">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-1065">Profile</span></span>

* <span data-ttu-id="b3904-1066">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1066">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b3904-1067">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b3904-1067">Service Fabric</span></span>

* <span data-ttu-id="b3904-1068">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-1068">Preview release</span></span>
* <span data-ttu-id="b3904-1069">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1069">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="b3904-1070">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1070">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="b3904-1071">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1071">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-1072">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1072">Storage</span></span>

* <span data-ttu-id="b3904-1073">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1073">Enabled setting blob tier</span></span>
* <span data-ttu-id="b3904-1074">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1074">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="b3904-1075">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1075">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="b3904-1076">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1076">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="b3904-1077">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1077">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="b3904-1078">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1078">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1079">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1079">VM</span></span>

* <span data-ttu-id="b3904-1080">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1080">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="b3904-1081">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1081">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="b3904-1082">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1082">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="b3904-1083">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1083">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="b3904-1084">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1084">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="b3904-1085">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1085">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="b3904-1086">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="b3904-1086">August 15, 2017</span></span>

<span data-ttu-id="b3904-1087">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="b3904-1087">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1088">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1088">ACS</span></span>

* <span data-ttu-id="b3904-1089">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1089">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1090">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-1090">Appservice</span></span>

* <span data-ttu-id="b3904-1091">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1091">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="b3904-1092">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b3904-1092">Event Grid</span></span>

* <span data-ttu-id="b3904-1093">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1093">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="b3904-1094">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="b3904-1094">August 11, 2017</span></span>

<span data-ttu-id="b3904-1095">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="b3904-1095">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1096">ACS</span></span>

* <span data-ttu-id="b3904-1097">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1097">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-1098">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-1098">Batch</span></span>

* <span data-ttu-id="b3904-1099">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1099">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="b3904-1100">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1100">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="b3904-1101">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1101">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="b3904-1102">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1102">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="b3904-1103">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1103">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="b3904-1104">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1104">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="b3904-1105">구성 요소</span><span class="sxs-lookup"><span data-stu-id="b3904-1105">Component</span></span>

* <span data-ttu-id="b3904-1106">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1106">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="b3904-1107">컨테이너</span><span class="sxs-lookup"><span data-stu-id="b3904-1107">Container</span></span>

* <span data-ttu-id="b3904-1108">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1108">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="b3904-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b3904-1109">Data Lake Store</span></span>

* <span data-ttu-id="b3904-1110">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1110">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="b3904-1111">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b3904-1111">Event Grid</span></span>

* <span data-ttu-id="b3904-1112">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-1112">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="b3904-1113">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-1113">Network</span></span>

* <span data-ttu-id="b3904-1114">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1114">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="b3904-1115">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1115">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="b3904-1116">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1116">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="b3904-1117">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1117">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-1118">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-1118">Profile</span></span>

* <span data-ttu-id="b3904-1119">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1119">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-1120">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1120">Storage</span></span>

* <span data-ttu-id="b3904-1121">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1121">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1122">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1122">VM</span></span>

* <span data-ttu-id="b3904-1123">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1123">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="b3904-1124">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1124">Exposed `list-skus` command</span></span>
* <span data-ttu-id="b3904-1125">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1125">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="b3904-1126">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1126">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="b3904-1127">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1127">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="b3904-1128">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="b3904-1128">July 28, 2017</span></span>

<span data-ttu-id="b3904-1129">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="b3904-1129">Version 2.0.12</span></span>

* <span data-ttu-id="b3904-1130">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1130">Added container commands</span></span>
* <span data-ttu-id="b3904-1131">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1131">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="b3904-1132">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-1132">Core</span></span>

* <span data-ttu-id="b3904-1133">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1133">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="b3904-1134">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1134">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="b3904-1135">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="b3904-1135">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="b3904-1136">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="b3904-1136">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="b3904-1137">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="b3904-1137">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="b3904-1138">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="b3904-1138">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="b3904-1139">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="b3904-1139">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b3904-1140">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="b3904-1140">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="b3904-1141">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="b3904-1141">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="b3904-1142">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="b3904-1142">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="b3904-1143">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="b3904-1143">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="b3904-1144">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="b3904-1144">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="b3904-1145">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1145">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="b3904-1146">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1146">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="b3904-1147">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1147">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="b3904-1148">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="b3904-1148">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="b3904-1149">ACR</span><span class="sxs-lookup"><span data-stu-id="b3904-1149">ACR</span></span>

* <span data-ttu-id="b3904-1150">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1150">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="b3904-1151">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1151">Support SKU update for managed registries</span></span>
* <span data-ttu-id="b3904-1152">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1152">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="b3904-1153">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1153">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="b3904-1154">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1154">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="b3904-1155">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1155">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1156">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1156">ACS</span></span>

* <span data-ttu-id="b3904-1157">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1157">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1158">App Service</span><span class="sxs-lookup"><span data-stu-id="b3904-1158">Appservice</span></span>

* <span data-ttu-id="b3904-1159">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1159">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="b3904-1160">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1160">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="b3904-1161">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1161">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="b3904-1162">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="b3904-1162">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="b3904-1163">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="b3904-1163">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="b3904-1164">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="b3904-1164">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="b3904-1165">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="b3904-1165">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="b3904-1166">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="b3904-1166">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="b3904-1167">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1167">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="b3904-1168">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1168">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="b3904-1169">Batch</span><span class="sxs-lookup"><span data-stu-id="b3904-1169">Batch</span></span>

* <span data-ttu-id="b3904-1170">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1170">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="b3904-1171">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1171">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="b3904-1172">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1172">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="b3904-1173">CDN</span><span class="sxs-lookup"><span data-stu-id="b3904-1173">CDN</span></span>

* <span data-ttu-id="b3904-1174">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1174">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="b3904-1175">클라우드</span><span class="sxs-lookup"><span data-stu-id="b3904-1175">Cloud</span></span>

* <span data-ttu-id="b3904-1176">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1176">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="b3904-1177">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1177">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="b3904-1178">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1178">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="b3904-1179">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1179">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="b3904-1180">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1180">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b3904-1181">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b3904-1181">CosmosDB</span></span>

* <span data-ttu-id="b3904-1182">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1182">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="b3904-1183">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1183">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b3904-1184">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b3904-1184">Data Lake Analytics</span></span>

* <span data-ttu-id="b3904-1185">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1185">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="b3904-1186">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1186">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="b3904-1187">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1187">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b3904-1188">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b3904-1188">Data Lake Store</span></span>

* <span data-ttu-id="b3904-1189">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1189">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="b3904-1190">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1190">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="b3904-1191">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1191">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="b3904-1192">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="b3904-1192">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="b3904-1193">대화형</span><span class="sxs-lookup"><span data-stu-id="b3904-1193">Interactive</span></span>

* <span data-ttu-id="b3904-1194">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1194">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="b3904-1195">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1195">Increased test coverage</span></span>
* <span data-ttu-id="b3904-1196">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1196">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="b3904-1197">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="b3904-1197">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="b3904-1198">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="b3904-1198">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="b3904-1199">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="b3904-1199">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="b3904-1200">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="b3904-1200">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b3904-1201">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1201">Added `--progress` flag</span></span>
* <span data-ttu-id="b3904-1202">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1202">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="b3904-1203">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="b3904-1203">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="b3904-1204">IoT</span><span class="sxs-lookup"><span data-stu-id="b3904-1204">IoT</span></span>

* <span data-ttu-id="b3904-1205">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1205">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="b3904-1206">(#3934)</span><span class="sxs-lookup"><span data-stu-id="b3904-1206">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="b3904-1207">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="b3904-1207">Key vault</span></span>

* <span data-ttu-id="b3904-1208">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="b3904-1208">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="b3904-1209">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b3904-1209">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="b3904-1210">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b3904-1210">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b3904-1211">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b3904-1211">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b3904-1212">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b3904-1212">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="b3904-1213">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="b3904-1213">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="b3904-1214">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1214">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="b3904-1215">(#3307)</span><span class="sxs-lookup"><span data-stu-id="b3904-1215">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="b3904-1216">랩</span><span class="sxs-lookup"><span data-stu-id="b3904-1216">Lab</span></span>

* <span data-ttu-id="b3904-1217">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1217">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="b3904-1218">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1218">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-1219">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-1219">Monitor</span></span>

* <span data-ttu-id="b3904-1220">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="b3904-1220">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="b3904-1221">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1221">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="b3904-1222">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1222">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="b3904-1223">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1223">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="b3904-1224">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1224">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="b3904-1225">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="b3904-1225">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="b3904-1226">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1226">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="b3904-1227">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1227">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="b3904-1228">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1228">`location` no longer required</span></span>
  * <span data-ttu-id="b3904-1229">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1229">Add name and ID support for target</span></span>
  * <span data-ttu-id="b3904-1230">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1230">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="b3904-1231">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1231">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="b3904-1232">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1232">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="b3904-1233">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1233">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="b3904-1234">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1234">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="b3904-1235">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1235">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="b3904-1236">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-1236">Network</span></span>

* <span data-ttu-id="b3904-1237">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1237">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="b3904-1238">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1238">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="b3904-1239">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1239">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="b3904-1240">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1240">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="b3904-1241">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1241">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="b3904-1242">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1242">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="b3904-1243">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="b3904-1243">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="b3904-1244">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="b3904-1244">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="b3904-1245">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="b3904-1245">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="b3904-1246">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b3904-1246">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="b3904-1247">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b3904-1247">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="b3904-1248">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="b3904-1248">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="b3904-1249">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="b3904-1249">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="b3904-1250">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b3904-1250">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="b3904-1251">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1251">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="b3904-1252">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1252">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="b3904-1253">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1253">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="b3904-1254">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1254">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="b3904-1255">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1255">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="b3904-1256">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1256">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="b3904-1257">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1257">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="b3904-1258">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1258">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="b3904-1259">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1259">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="b3904-1260">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1260">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="b3904-1261">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1261">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="b3904-1262">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1262">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="b3904-1263">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1263">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-1264">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-1264">Profile</span></span>

* <span data-ttu-id="b3904-1265">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1265">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="b3904-1266">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1266">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="b3904-1267">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1267">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="b3904-1268">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1268">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="b3904-1269">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1269">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="b3904-1270">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b3904-1270">RDBMS</span></span>

* <span data-ttu-id="b3904-1271">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="b3904-1271">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="b3904-1272">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="b3904-1272">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="b3904-1273">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="b3904-1273">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="b3904-1274">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="b3904-1274">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-1275">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-1275">Resource</span></span>

* <span data-ttu-id="b3904-1276">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1276">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="b3904-1277">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1277">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="b3904-1278">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1278">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="b3904-1279">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1279">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="b3904-1280">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="b3904-1280">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="b3904-1281">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1281">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="b3904-1282">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="b3904-1282">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="b3904-1283">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1283">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="b3904-1284">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-1284">Role</span></span>

* <span data-ttu-id="b3904-1285">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1285">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="b3904-1286">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="b3904-1286">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="b3904-1287">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1287">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="b3904-1288">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1288">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="b3904-1289">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1289">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b3904-1290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b3904-1290">Service Fabric</span></span>
* <span data-ttu-id="b3904-1291">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="b3904-1291">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="b3904-1292">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="b3904-1292">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="b3904-1293">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="b3904-1293">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-1294">SQL</span></span>

* <span data-ttu-id="b3904-1295">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1295">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="b3904-1296">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1296">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="b3904-1297">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1297">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-1298">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1298">Storage</span></span>

* <span data-ttu-id="b3904-1299">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="b3904-1299">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="b3904-1300">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="b3904-1300">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="b3904-1301">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="b3904-1301">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="b3904-1302">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1302">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="b3904-1303">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="b3904-1303">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="b3904-1304">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="b3904-1304">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1305">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1305">VM</span></span>

* <span data-ttu-id="b3904-1306">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1306">Support configuring nsg</span></span>
* <span data-ttu-id="b3904-1307">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1307">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="b3904-1308">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1308">Support managed service identities</span></span>
* <span data-ttu-id="b3904-1309">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1309">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="b3904-1310">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1310">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="b3904-1311">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="b3904-1311">May 10, 2017</span></span>

<span data-ttu-id="b3904-1312">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="b3904-1312">Version 2.0.6</span></span>

* <span data-ttu-id="b3904-1313">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="b3904-1313">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="b3904-1314">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1314">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="b3904-1315">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="b3904-1315">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="b3904-1316">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="b3904-1316">Include Cognitive Services module</span></span>
* <span data-ttu-id="b3904-1317">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="b3904-1317">Include Service Fabric module</span></span>
* <span data-ttu-id="b3904-1318">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="b3904-1318">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="b3904-1319">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1319">Add support for CDN commands</span></span>
* <span data-ttu-id="b3904-1320">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-1320">Remove Container module</span></span>
* <span data-ttu-id="b3904-1321">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="b3904-1321">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="b3904-1322">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b3904-1322">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="b3904-1323">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-1323">Core</span></span>

* <span data-ttu-id="b3904-1324">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="b3904-1324">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="b3904-1325">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="b3904-1325">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="b3904-1326">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="b3904-1326">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="b3904-1327">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="b3904-1327">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="b3904-1328">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="b3904-1328">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="b3904-1329">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="b3904-1329">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="b3904-1330">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="b3904-1330">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="b3904-1331">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="b3904-1331">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="b3904-1332">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="b3904-1332">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="b3904-1333">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="b3904-1333">core: Improved performance</span></span>
* <span data-ttu-id="b3904-1334">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1334">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="b3904-1335">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="b3904-1335">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1336">ACS</span></span>

* <span data-ttu-id="b3904-1337">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1337">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="b3904-1338">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="b3904-1338">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="b3904-1339">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="b3904-1339">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="b3904-1340">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="b3904-1340">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1341">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-1341">AppService</span></span>

* <span data-ttu-id="b3904-1342">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="b3904-1342">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="b3904-1343">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1343">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="b3904-1344">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="b3904-1344">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="b3904-1345">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="b3904-1345">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="b3904-1346">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="b3904-1346">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="b3904-1347">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="b3904-1347">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="b3904-1348">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1348">support slot swap with preview</span></span>
* <span data-ttu-id="b3904-1349">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="b3904-1349">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="b3904-1350">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="b3904-1350">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b3904-1351">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b3904-1351">CosmosDB</span></span>

* <span data-ttu-id="b3904-1352">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="b3904-1352">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="b3904-1353">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1353">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="b3904-1354">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1354">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="b3904-1355">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1355">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b3904-1356">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b3904-1356">Data Lake Analytics</span></span>

* <span data-ttu-id="b3904-1357">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1357">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="b3904-1358">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1358">Add support for new catalog item type: package.</span></span> <span data-ttu-id="b3904-1359">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="b3904-1359">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="b3904-1360">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="b3904-1360">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="b3904-1361">테이블</span><span class="sxs-lookup"><span data-stu-id="b3904-1361">Table</span></span>
  * <span data-ttu-id="b3904-1362">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="b3904-1362">Table valued function</span></span>
  * <span data-ttu-id="b3904-1363">보기</span><span class="sxs-lookup"><span data-stu-id="b3904-1363">View</span></span>
  * <span data-ttu-id="b3904-1364">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="b3904-1364">Table Statistics.</span></span> <span data-ttu-id="b3904-1365">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="b3904-1365">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b3904-1366">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b3904-1366">Data Lake Store</span></span>

* <span data-ttu-id="b3904-1367">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="b3904-1367">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="b3904-1368">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b3904-1368">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="b3904-1369">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="b3904-1369">missed help for access show.</span></span> <span data-ttu-id="b3904-1370">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1370">adding it.</span></span> <span data-ttu-id="b3904-1371">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="b3904-1371">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="b3904-1372">찾기</span><span class="sxs-lookup"><span data-stu-id="b3904-1372">Find</span></span>

* <span data-ttu-id="b3904-1373">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="b3904-1373">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="b3904-1374">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b3904-1374">KeyVault</span></span>

* <span data-ttu-id="b3904-1375">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1375">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="b3904-1376">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1376">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="b3904-1377">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1377">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="b3904-1378">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1378">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="b3904-1379">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="b3904-1379">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="b3904-1380">랩</span><span class="sxs-lookup"><span data-stu-id="b3904-1380">Lab</span></span>

* <span data-ttu-id="b3904-1381">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1381">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="b3904-1382">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1382">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="b3904-1383">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="b3904-1383">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="b3904-1384">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="b3904-1384">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="b3904-1385">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1385">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="b3904-1386">모니터</span><span class="sxs-lookup"><span data-stu-id="b3904-1386">Monitor</span></span>

* <span data-ttu-id="b3904-1387">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="b3904-1387">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="b3904-1388">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="b3904-1388">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="b3904-1389">네트워크</span><span class="sxs-lookup"><span data-stu-id="b3904-1389">Network</span></span>

* <span data-ttu-id="b3904-1390">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1390">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="b3904-1391">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1391">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="b3904-1392">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1392">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="b3904-1393">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1393">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="b3904-1394">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1394">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="b3904-1395">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1395">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="b3904-1396">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1396">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="b3904-1397">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1397">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="b3904-1398">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1398">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="b3904-1399">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1399">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="b3904-1400">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="b3904-1400">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="b3904-1401">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1401">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="b3904-1402">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1402">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="b3904-1403">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1403">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="b3904-1404">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="b3904-1404">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="b3904-1405">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1405">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="b3904-1406">프로필</span><span class="sxs-lookup"><span data-stu-id="b3904-1406">Profile</span></span>

* <span data-ttu-id="b3904-1407">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="b3904-1407">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="b3904-1408">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="b3904-1408">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="b3904-1409">Redis</span><span class="sxs-lookup"><span data-stu-id="b3904-1409">Redis</span></span>

* <span data-ttu-id="b3904-1410">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1410">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="b3904-1411">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="b3904-1411">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="b3904-1412">리소스</span><span class="sxs-lookup"><span data-stu-id="b3904-1412">Resource</span></span>

* <span data-ttu-id="b3904-1413">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="b3904-1413">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="b3904-1414">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="b3904-1414">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="b3904-1415">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="b3904-1415">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="b3904-1416">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1416">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="b3904-1417">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="b3904-1417">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="b3904-1418">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1418">Add docs for az lock update.</span></span> <span data-ttu-id="b3904-1419">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="b3904-1419">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="b3904-1420">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1420">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="b3904-1421">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="b3904-1421">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="b3904-1422">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1422">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="b3904-1423">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="b3904-1423">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="b3904-1424">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="b3904-1424">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="b3904-1425">역할</span><span class="sxs-lookup"><span data-stu-id="b3904-1425">Role</span></span>

* <span data-ttu-id="b3904-1426">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="b3904-1426">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="b3904-1427">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="b3904-1427">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="b3904-1428">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="b3904-1428">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="b3904-1429">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="b3904-1429">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="b3904-1430">SQL</span><span class="sxs-lookup"><span data-stu-id="b3904-1430">SQL</span></span>

* <span data-ttu-id="b3904-1431">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="b3904-1431">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="b3904-1432">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="b3904-1432">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="b3904-1433">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1433">Storage</span></span>

* <span data-ttu-id="b3904-1434">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="b3904-1434">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="b3904-1435">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1435">Add support for incremental blob copy</span></span>
* <span data-ttu-id="b3904-1436">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1436">Add support for large block blob upload</span></span>
* <span data-ttu-id="b3904-1437">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="b3904-1437">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1438">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1438">VM</span></span>

* <span data-ttu-id="b3904-1439">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="b3904-1439">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="b3904-1440">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="b3904-1440">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="b3904-1441">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="b3904-1441">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="b3904-1442">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="b3904-1442">az vm/vmss disk</span></span>
  3. <span data-ttu-id="b3904-1443">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1443">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="b3904-1444">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="b3904-1444">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="b3904-1445">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="b3904-1445">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="b3904-1446">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="b3904-1446">April 3, 2017</span></span>

<span data-ttu-id="b3904-1447">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="b3904-1447">Version 2.0.2</span></span>

<span data-ttu-id="b3904-1448">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1448">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="b3904-1449">코어</span><span class="sxs-lookup"><span data-stu-id="b3904-1449">Core</span></span>

* <span data-ttu-id="b3904-1450">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="b3904-1450">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="b3904-1451">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="b3904-1451">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="b3904-1452">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="b3904-1452">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="b3904-1453">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b3904-1453">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b3904-1454">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="b3904-1454">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="b3904-1455">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="b3904-1455">Add prompting for missing template parameters.</span></span> <span data-ttu-id="b3904-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="b3904-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="b3904-1457">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1457">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="b3904-1458">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="b3904-1458">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="b3904-1459">ACS</span><span class="sxs-lookup"><span data-stu-id="b3904-1459">ACS</span></span>

* <span data-ttu-id="b3904-1460">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="b3904-1460">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="b3904-1461">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="b3904-1461">Add support for ssh key password prompting.</span></span> <span data-ttu-id="b3904-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="b3904-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="b3904-1463">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="b3904-1463">Add support for windows clusters.</span></span> <span data-ttu-id="b3904-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="b3904-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="b3904-1465">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="b3904-1465">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="b3904-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="b3904-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="b3904-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="b3904-1467">AppService</span></span>

* <span data-ttu-id="b3904-1468">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="b3904-1468">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="b3904-1469">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="b3904-1469">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="b3904-1470">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="b3904-1470">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="b3904-1471">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="b3904-1471">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="b3904-1472">DataLake</span><span class="sxs-lookup"><span data-stu-id="b3904-1472">DataLake</span></span>

* <span data-ttu-id="b3904-1473">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-1473">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="b3904-1474">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="b3904-1474">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="b3904-1475">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="b3904-1475">DocuemntDB</span></span>

* <span data-ttu-id="b3904-1476">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="b3904-1476">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="b3904-1477">VM</span><span class="sxs-lookup"><span data-stu-id="b3904-1477">VM</span></span>

* <span data-ttu-id="b3904-1478">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="b3904-1478">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="b3904-1479">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="b3904-1479">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="b3904-1480">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="b3904-1480">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="b3904-1481">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b3904-1481">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b3904-1482">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="b3904-1482">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="b3904-1483">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="b3904-1483">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="b3904-1484">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="b3904-1484">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="b3904-1485">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="b3904-1485">February 27, 2017</span></span>

<span data-ttu-id="b3904-1486">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="b3904-1486">Version 2.0.0</span></span>

<span data-ttu-id="b3904-1487">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1487">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="b3904-1488">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="b3904-1488">Container Service (acs)</span></span>
- <span data-ttu-id="b3904-1489">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="b3904-1489">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="b3904-1490">네트워킹</span><span class="sxs-lookup"><span data-stu-id="b3904-1490">Networking</span></span>
- <span data-ttu-id="b3904-1491">Storage</span><span class="sxs-lookup"><span data-stu-id="b3904-1491">Storage</span></span>

<span data-ttu-id="b3904-1492">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1492">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="b3904-1493">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1493">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="b3904-1494">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1494">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="b3904-1495">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1495">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="b3904-1496">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3904-1496">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="b3904-1497">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3904-1497">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="b3904-1498">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="b3904-1498">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="b3904-1499">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="b3904-1499">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="b3904-1500">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="b3904-1500">Provide feedback from the command line with the `az feedback` command</span></span>


---
title: Azure CLI 2.0 릴리스 정보
description: Azure CLI 2.0 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="15ea2-103">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="15ea2-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="15ea2-104">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="15ea2-104">March 27, 2018</span></span>

<span data-ttu-id="15ea2-105">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="15ea2-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-106">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-106">Core</span></span>

* <span data-ttu-id="15ea2-107">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="15ea2-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-108">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-108">ACS</span></span>

* <span data-ttu-id="15ea2-109">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-110">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-110">Appservice</span></span>

* <span data-ttu-id="15ea2-111">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="15ea2-112">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15ea2-113">Backup</span><span class="sxs-lookup"><span data-stu-id="15ea2-113">Backup</span></span>

* <span data-ttu-id="15ea2-114">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="15ea2-115">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="15ea2-116">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="15ea2-117">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-118">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-118">Container</span></span>

* <span data-ttu-id="15ea2-119">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-119">Added `container exec` command.</span></span> <span data-ttu-id="15ea2-120">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="15ea2-121">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="15ea2-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="15ea2-122">확장</span><span class="sxs-lookup"><span data-stu-id="15ea2-122">Extension</span></span>

* <span data-ttu-id="15ea2-123">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="15ea2-124">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="15ea2-125">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-126">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-126">Interactive</span></span>

* <span data-ttu-id="15ea2-127">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="15ea2-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="15ea2-128">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="15ea2-129">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="15ea2-130">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="15ea2-131">랩</span><span class="sxs-lookup"><span data-stu-id="15ea2-131">Lab</span></span>

* <span data-ttu-id="15ea2-132">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-133">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-133">Monitor</span></span>

* <span data-ttu-id="15ea2-134">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="15ea2-135">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="15ea2-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="15ea2-136">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-137">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-137">Network</span></span>

* <span data-ttu-id="15ea2-138">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-139">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-139">Profile</span></span>

* <span data-ttu-id="15ea2-140">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ea2-141">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ea2-141">RDBMS</span></span>

* <span data-ttu-id="15ea2-142">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-143">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-143">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="15ea2-145">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-145">Role</span></span>

* <span data-ttu-id="15ea2-146">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="15ea2-147">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="15ea2-148">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="15ea2-149">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="15ea2-150">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-151">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-151">Storage</span></span>

* <span data-ttu-id="15ea2-152">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="15ea2-153">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="15ea2-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-154">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-154">VM</span></span>

* <span data-ttu-id="15ea2-155">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="15ea2-156">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="15ea2-157">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="15ea2-158">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="15ea2-159">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="15ea2-159">March 13, 2018</span></span>

<span data-ttu-id="15ea2-160">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="15ea2-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="15ea2-161">ACR</span><span class="sxs-lookup"><span data-stu-id="15ea2-161">ACR</span></span>

* <span data-ttu-id="15ea2-162">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="15ea2-163">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="15ea2-164">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-165">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-165">ACS</span></span>

* <span data-ttu-id="15ea2-166">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="15ea2-167">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="15ea2-168">Advisor</span><span class="sxs-lookup"><span data-stu-id="15ea2-168">Advisor</span></span>

* <span data-ttu-id="15ea2-169">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="15ea2-170">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="15ea2-171">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="15ea2-172">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="15ea2-173">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-174">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-174">Appservice</span></span>

* <span data-ttu-id="15ea2-175">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="15ea2-176">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="15ea2-177">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="15ea2-177">Eventhubs</span></span>

* <span data-ttu-id="15ea2-178">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="15ea2-179">내선 번호</span><span class="sxs-lookup"><span data-stu-id="15ea2-179">Extension</span></span>

* <span data-ttu-id="15ea2-180">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-181">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-181">Interactive</span></span>

* <span data-ttu-id="15ea2-182">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="15ea2-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="15ea2-183">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="15ea2-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="15ea2-184">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="15ea2-185">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-186">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-186">Monitor</span></span>

* <span data-ttu-id="15ea2-187">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="15ea2-188">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="15ea2-189">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="15ea2-190">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-191">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-191">Network</span></span>

* <span data-ttu-id="15ea2-192">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="15ea2-193">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="15ea2-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="15ea2-194">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="15ea2-195">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-196">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-196">Profile</span></span>

* <span data-ttu-id="15ea2-197">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="15ea2-198">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ea2-199">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ea2-199">RDBMS</span></span>

* <span data-ttu-id="15ea2-200">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ea2-201">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ea2-201">Service Bus</span></span>

* <span data-ttu-id="15ea2-202">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-203">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-203">Storage</span></span>

* <span data-ttu-id="15ea2-204">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="15ea2-205">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-206">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-206">VM</span></span>

* <span data-ttu-id="15ea2-207">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="15ea2-208">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="15ea2-209">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="15ea2-210">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="15ea2-211">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="15ea2-211">February 27, 2018</span></span>

<span data-ttu-id="15ea2-212">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="15ea2-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-213">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-213">Core</span></span>

* <span data-ttu-id="15ea2-214">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="15ea2-215">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="15ea2-216">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-217">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-217">ACS</span></span>

* <span data-ttu-id="15ea2-218">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="15ea2-219">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="15ea2-220">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="15ea2-221">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="15ea2-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-222">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-222">Appservice</span></span>

* <span data-ttu-id="15ea2-223">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="15ea2-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="15ea2-224">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ea2-225">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ea2-225">Cognitive Services</span></span>

* <span data-ttu-id="15ea2-226">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="15ea2-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="15ea2-227">Consumption</span><span class="sxs-lookup"><span data-stu-id="15ea2-227">Consumption</span></span>

* <span data-ttu-id="15ea2-228">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="15ea2-229">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="15ea2-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-230">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-230">Container</span></span>

* <span data-ttu-id="15ea2-231">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-232">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-232">Network</span></span>

* <span data-ttu-id="15ea2-233">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-234">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-234">Resource</span></span>

* <span data-ttu-id="15ea2-235">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-236">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-236">Role</span></span>

* <span data-ttu-id="15ea2-237">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-238">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-238">SQL</span></span>

* <span data-ttu-id="15ea2-239">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-240">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-240">Storage</span></span>

* <span data-ttu-id="15ea2-241">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="15ea2-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-242">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-242">VM</span></span>

* <span data-ttu-id="15ea2-243">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="15ea2-244">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="15ea2-244">February 13, 2018</span></span>

<span data-ttu-id="15ea2-245">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="15ea2-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-246">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-246">Core</span></span>

* <span data-ttu-id="15ea2-247">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-248">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-248">ACS</span></span>

* <span data-ttu-id="15ea2-249">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="15ea2-250">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="15ea2-251">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="15ea2-252">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="15ea2-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="15ea2-253">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="15ea2-254">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="15ea2-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="15ea2-255">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="15ea2-256">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-257">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-257">Appservice</span></span>

* <span data-ttu-id="15ea2-258">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="15ea2-259">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="15ea2-260">CDN</span><span class="sxs-lookup"><span data-stu-id="15ea2-260">CDN</span></span>

* <span data-ttu-id="15ea2-261">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-262">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-262">Container</span></span>

* <span data-ttu-id="15ea2-263">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="15ea2-264">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ea2-265">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ea2-265">CosmosDB</span></span>

* <span data-ttu-id="15ea2-266">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="15ea2-267">내선 번호</span><span class="sxs-lookup"><span data-stu-id="15ea2-267">Extension</span></span>

* <span data-ttu-id="15ea2-268">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="15ea2-269">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="15ea2-270">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="15ea2-270">Feedback</span></span>

* <span data-ttu-id="15ea2-271">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-272">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-272">Interactive</span></span>

* <span data-ttu-id="15ea2-273">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="15ea2-274">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="15ea2-275">IoT</span><span class="sxs-lookup"><span data-stu-id="15ea2-275">IoT</span></span>

* <span data-ttu-id="15ea2-276">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15ea2-277">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15ea2-278">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="15ea2-279">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-280">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-280">Monitor</span></span>

* <span data-ttu-id="15ea2-281">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-282">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-282">Network</span></span>

* <span data-ttu-id="15ea2-283">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="15ea2-284">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-284">Profile</span></span>

* <span data-ttu-id="15ea2-285">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-286">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-286">Resource</span></span>

* <span data-ttu-id="15ea2-287">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-288">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-288">Role</span></span>

* <span data-ttu-id="15ea2-289">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-290">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-290">SQL</span></span>

* <span data-ttu-id="15ea2-291">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="15ea2-292">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-292">Added `sql db rename`</span></span>
* <span data-ttu-id="15ea2-293">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-294">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-294">Storage</span></span>

* <span data-ttu-id="15ea2-295">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-296">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-296">VM</span></span>

* <span data-ttu-id="15ea2-297">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="15ea2-298">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="15ea2-299">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="15ea2-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="15ea2-300">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="15ea2-300">January 31, 2018</span></span>

<span data-ttu-id="15ea2-301">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="15ea2-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-302">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-302">Core</span></span>

* <span data-ttu-id="15ea2-303">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="15ea2-304">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="15ea2-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="15ea2-305">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="15ea2-306">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="15ea2-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="15ea2-307">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-308">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-308">ACS</span></span>

* <span data-ttu-id="15ea2-309">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="15ea2-310">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="15ea2-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-311">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-311">Appservice</span></span>

* <span data-ttu-id="15ea2-312">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="15ea2-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="15ea2-313">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="15ea2-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="15ea2-314">CDN</span><span class="sxs-lookup"><span data-stu-id="15ea2-314">CDN</span></span>

* <span data-ttu-id="15ea2-315">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ea2-316">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ea2-316">CosmosDB</span></span>

* <span data-ttu-id="15ea2-317">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-318">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-318">Interactive</span></span>

* <span data-ttu-id="15ea2-319">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-320">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-320">Network</span></span>

* <span data-ttu-id="15ea2-321">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="15ea2-322">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="15ea2-323">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="15ea2-324">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="15ea2-325">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="15ea2-326">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="15ea2-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="15ea2-327">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="15ea2-328">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="15ea2-329">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="15ea2-330">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="15ea2-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-331">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-331">Profile</span></span>

* <span data-ttu-id="15ea2-332">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-333">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-333">Resource</span></span>

* <span data-ttu-id="15ea2-334">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-335">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-335">Storage</span></span>

* <span data-ttu-id="15ea2-336">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="15ea2-337">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="15ea2-338">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="15ea2-339">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="15ea2-340">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-341">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-341">VM</span></span>

* <span data-ttu-id="15ea2-342">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="15ea2-343">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="15ea2-344">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="15ea2-345">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="15ea2-346">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="15ea2-346">January 17, 2018</span></span>

<span data-ttu-id="15ea2-347">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="15ea2-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="15ea2-348">ACR</span><span class="sxs-lookup"><span data-stu-id="15ea2-348">ACR</span></span>

* <span data-ttu-id="15ea2-349">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="15ea2-350">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-351">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-351">ACS</span></span>

* <span data-ttu-id="15ea2-352">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="15ea2-353">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-354">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-354">Appservice</span></span>

* <span data-ttu-id="15ea2-355">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="15ea2-356">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="15ea2-357">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="15ea2-358">Backup</span><span class="sxs-lookup"><span data-stu-id="15ea2-358">Backup</span></span>

* <span data-ttu-id="15ea2-359">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="15ea2-360">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="15ea2-361">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="15ea2-362">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="15ea2-363">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="15ea2-364">Batch</span><span class="sxs-lookup"><span data-stu-id="15ea2-364">Batch</span></span>

* <span data-ttu-id="15ea2-365">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="15ea2-366">클라우드</span><span class="sxs-lookup"><span data-stu-id="15ea2-366">Cloud</span></span>

* <span data-ttu-id="15ea2-367">클라우드에서 `--profile`을 설정할 때 끝점을 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="15ea2-368">Consumption</span><span class="sxs-lookup"><span data-stu-id="15ea2-368">Consumption</span></span>

* <span data-ttu-id="15ea2-369">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ea2-370">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ea2-370">Event Grid</span></span>

* <span data-ttu-id="15ea2-371">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15ea2-372">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15ea2-373">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="15ea2-374">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="15ea2-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="15ea2-375">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="15ea2-376">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="15ea2-377">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="15ea2-378">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-379">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-379">Interactive</span></span>

* <span data-ttu-id="15ea2-380">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="15ea2-381">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-381">Fixed errors on startup</span></span>
* <span data-ttu-id="15ea2-382">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="15ea2-383">IoT</span><span class="sxs-lookup"><span data-stu-id="15ea2-383">IoT</span></span>

* <span data-ttu-id="15ea2-384">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="15ea2-385">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="15ea2-386">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-387">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-387">Monitor</span></span>

* <span data-ttu-id="15ea2-388">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="15ea2-389">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="15ea2-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="15ea2-390">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-391">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-391">Network</span></span>

* <span data-ttu-id="15ea2-392">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="15ea2-393">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-394">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-394">Profile</span></span>

* <span data-ttu-id="15ea2-395">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-396">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-396">Role</span></span>

* <span data-ttu-id="15ea2-397">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ea2-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ea2-398">Service Fabric</span></span>

* <span data-ttu-id="15ea2-399">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="15ea2-400">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-401">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-401">VM</span></span>

* <span data-ttu-id="15ea2-402">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="15ea2-403">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="15ea2-404">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="15ea2-405">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="15ea2-406">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="15ea2-407">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ea2-408">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ea2-409">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="15ea2-410">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="15ea2-410">December 19, 2017</span></span>

<span data-ttu-id="15ea2-411">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="15ea2-411">Version 2.0.23</span></span>

* <span data-ttu-id="15ea2-412">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-413">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-413">Container</span></span>

* <span data-ttu-id="15ea2-414">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-415">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-415">Network</span></span>

* <span data-ttu-id="15ea2-416">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="15ea2-417">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-418">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-418">Storage</span></span>

* <span data-ttu-id="15ea2-419">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-420">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-420">VM</span></span>

* <span data-ttu-id="15ea2-421">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="15ea2-422">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="15ea2-422">December 5, 2017</span></span>

<span data-ttu-id="15ea2-423">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="15ea2-423">Version 2.0.22</span></span>

* <span data-ttu-id="15ea2-424">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-424">Removed `az component` commands.</span></span> <span data-ttu-id="15ea2-425">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="15ea2-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-426">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-426">Core</span></span>
* <span data-ttu-id="15ea2-427">`AZURE_US_GOV_CLOUD` AAD 권한 끝점이 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="15ea2-428">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-429">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-429">ACS</span></span>

* <span data-ttu-id="15ea2-430">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="15ea2-431">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="15ea2-432">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="15ea2-433">Advisor</span><span class="sxs-lookup"><span data-stu-id="15ea2-433">Advisor</span></span>

* <span data-ttu-id="15ea2-434">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-435">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-435">Appservice</span></span>

* <span data-ttu-id="15ea2-436">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="15ea2-437">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="15ea2-438">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="15ea2-439">Consumption</span><span class="sxs-lookup"><span data-stu-id="15ea2-439">Consumption</span></span>

* <span data-ttu-id="15ea2-440">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-441">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-441">Container</span></span>

* <span data-ttu-id="15ea2-442">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-443">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-443">Monitor</span></span>

* <span data-ttu-id="15ea2-444">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-445">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-445">Resource</span></span>

* <span data-ttu-id="15ea2-446">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-447">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-447">Role</span></span>

* <span data-ttu-id="15ea2-448">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="15ea2-449">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="15ea2-450">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-451">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-451">SQL</span></span>

* <span data-ttu-id="15ea2-452">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="15ea2-453">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-454">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-454">VM</span></span>

* <span data-ttu-id="15ea2-455">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="15ea2-456">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="15ea2-456">November 14, 2017</span></span>

<span data-ttu-id="15ea2-457">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="15ea2-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="15ea2-458">ACR</span><span class="sxs-lookup"><span data-stu-id="15ea2-458">ACR</span></span>

* <span data-ttu-id="15ea2-459">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="15ea2-460">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-460">ACS</span></span>

* <span data-ttu-id="15ea2-461">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="15ea2-462">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="15ea2-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="15ea2-463">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="15ea2-464">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="15ea2-465">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-466">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-466">Appservice</span></span>

* <span data-ttu-id="15ea2-467">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="15ea2-468">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="15ea2-469">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="15ea2-470">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="15ea2-471">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="15ea2-472">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="15ea2-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="15ea2-473">Batch</span><span class="sxs-lookup"><span data-stu-id="15ea2-473">Batch</span></span>

* <span data-ttu-id="15ea2-474">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="15ea2-475">Batchai</span><span class="sxs-lookup"><span data-stu-id="15ea2-475">Batchai</span></span>

* <span data-ttu-id="15ea2-476">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="15ea2-477">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="15ea2-478">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="15ea2-479">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="15ea2-480">클라우드</span><span class="sxs-lookup"><span data-stu-id="15ea2-480">Cloud</span></span>

* <span data-ttu-id="15ea2-481">필요한 끝점이 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-482">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-482">Container</span></span>

* <span data-ttu-id="15ea2-483">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="15ea2-484">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-484">Added container group restart policy</span></span>
* <span data-ttu-id="15ea2-485">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="15ea2-486">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="15ea2-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ea2-487">Data Lake Analytics
</span><span class="sxs-lookup"><span data-stu-id="15ea2-487">Data Lake Analytics</span></span>

* <span data-ttu-id="15ea2-488">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ea2-489">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ea2-489">Data Lake Store</span></span>

* <span data-ttu-id="15ea2-490">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="15ea2-491">내선 번호</span><span class="sxs-lookup"><span data-stu-id="15ea2-491">Extension</span></span>

* <span data-ttu-id="15ea2-492">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="15ea2-493">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="15ea2-494">IoT</span><span class="sxs-lookup"><span data-stu-id="15ea2-494">IoT</span></span>

* <span data-ttu-id="15ea2-495">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-496">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-496">Monitor</span></span>

* <span data-ttu-id="15ea2-497">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-498">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-498">Network</span></span>

* <span data-ttu-id="15ea2-499">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="15ea2-500">`traffic-manager profile update`로 끝점을 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="15ea2-501">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="15ea2-502">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="15ea2-503">예약</span><span class="sxs-lookup"><span data-stu-id="15ea2-503">Reservations</span></span>

* <span data-ttu-id="15ea2-504">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-505">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-505">Resource</span></span>

* <span data-ttu-id="15ea2-506">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-507">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-507">SQL</span></span>

* <span data-ttu-id="15ea2-508">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-509">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-509">Storage</span></span>

* <span data-ttu-id="15ea2-510">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="15ea2-511">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="15ea2-512">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="15ea2-513">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="15ea2-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="15ea2-514">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="15ea2-515">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="15ea2-516">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-517">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-517">VM</span></span>

* <span data-ttu-id="15ea2-518">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="15ea2-519">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="15ea2-520">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="15ea2-521">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="15ea2-522">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="15ea2-523">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="15ea2-523">October 24, 2017</span></span>

<span data-ttu-id="15ea2-524">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="15ea2-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-525">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-525">Core</span></span>

* <span data-ttu-id="15ea2-526">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="15ea2-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="15ea2-527">ACR</span><span class="sxs-lookup"><span data-stu-id="15ea2-527">ACR</span></span>

* <span data-ttu-id="15ea2-528">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="15ea2-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="15ea2-529">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="15ea2-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="15ea2-530">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="15ea2-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-531">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-531">ACS</span></span>

* <span data-ttu-id="15ea2-532">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="15ea2-533">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-534">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-534">Appservice</span></span>

* <span data-ttu-id="15ea2-535">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="15ea2-536">구성 요소</span><span class="sxs-lookup"><span data-stu-id="15ea2-536">Component</span></span>

* <span data-ttu-id="15ea2-537">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-538">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-538">Monitor</span></span>

* <span data-ttu-id="15ea2-539">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-540">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-540">Resource</span></span>

* <span data-ttu-id="15ea2-541">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="15ea2-542">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-543">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-543">VM</span></span>

* <span data-ttu-id="15ea2-544">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="15ea2-545">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="15ea2-545">October 9, 2017</span></span>

<span data-ttu-id="15ea2-546">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="15ea2-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-547">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-547">Core</span></span>

* <span data-ttu-id="15ea2-548">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-549">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-549">Appservice</span></span>

* <span data-ttu-id="15ea2-550">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="15ea2-551">Batch</span><span class="sxs-lookup"><span data-stu-id="15ea2-551">Batch</span></span>

* <span data-ttu-id="15ea2-552">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="15ea2-553">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="15ea2-554">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="15ea2-555">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="15ea2-556">Batchai</span><span class="sxs-lookup"><span data-stu-id="15ea2-556">Batchai</span></span>

* <span data-ttu-id="15ea2-557">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ea2-558">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15ea2-558">Keyvault</span></span>

* <span data-ttu-id="15ea2-559">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="15ea2-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="15ea2-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="15ea2-561">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-561">Network</span></span>

* <span data-ttu-id="15ea2-562">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="15ea2-563">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-564">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-564">Resource</span></span>

* <span data-ttu-id="15ea2-565">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="15ea2-566">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="15ea2-567">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="15ea2-568">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-569">Sql</span><span class="sxs-lookup"><span data-stu-id="15ea2-569">Sql</span></span>

* <span data-ttu-id="15ea2-570">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="15ea2-571">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="15ea2-572">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-573">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-573">Storage</span></span>

* <span data-ttu-id="15ea2-574">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-575">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-575">Vm</span></span>

* <span data-ttu-id="15ea2-576">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="15ea2-577">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="15ea2-578">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="15ea2-579">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="15ea2-580">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="15ea2-581">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="15ea2-581">September 22, 2017</span></span>

<span data-ttu-id="15ea2-582">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="15ea2-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-583">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-583">Resource</span></span>

* <span data-ttu-id="15ea2-584">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="15ea2-585">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="15ea2-586">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="15ea2-587">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-588">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-588">Network</span></span>

* <span data-ttu-id="15ea2-589">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="15ea2-590">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="15ea2-591">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="15ea2-592">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="15ea2-593">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15ea2-594">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="15ea2-595">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-596">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-596">Storage</span></span>

* <span data-ttu-id="15ea2-597">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ea2-598">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ea2-598">Eventgrid</span></span>

* <span data-ttu-id="15ea2-599">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="15ea2-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-600">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-600">SQL</span></span>

* <span data-ttu-id="15ea2-601">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="15ea2-602">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="15ea2-603">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ea2-604">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15ea2-604">Keyvault</span></span>

* <span data-ttu-id="15ea2-605">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-606">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-606">VM</span></span>

* <span data-ttu-id="15ea2-607">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="15ea2-608">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15ea2-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="15ea2-609">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="15ea2-610">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="15ea2-611">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="15ea2-612">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-613">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-613">ACS</span></span>

* <span data-ttu-id="15ea2-614">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-615">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-615">Appservice</span></span>

* <span data-ttu-id="15ea2-616">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15ea2-617">Backup</span><span class="sxs-lookup"><span data-stu-id="15ea2-617">Backup</span></span>

* <span data-ttu-id="15ea2-618">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="15ea2-619">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="15ea2-619">September 11, 2017</span></span>

<span data-ttu-id="15ea2-620">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="15ea2-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="15ea2-621">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-621">Core</span></span>

* <span data-ttu-id="15ea2-622">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="15ea2-623">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-624">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-624">Acs</span></span>

* <span data-ttu-id="15ea2-625">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="15ea2-626">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="15ea2-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-627">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-627">Appservice</span></span>

* <span data-ttu-id="15ea2-628">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="15ea2-629">CDN</span><span class="sxs-lookup"><span data-stu-id="15ea2-629">CDN</span></span>

* <span data-ttu-id="15ea2-630">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="15ea2-631">확장</span><span class="sxs-lookup"><span data-stu-id="15ea2-631">Extension</span></span>

* <span data-ttu-id="15ea2-632">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ea2-633">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15ea2-633">Keyvault</span></span>

* <span data-ttu-id="15ea2-634">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-635">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-635">Network</span></span>

* <span data-ttu-id="15ea2-636">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15ea2-637">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="15ea2-638">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="15ea2-639">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15ea2-640">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-641">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-641">Resource</span></span>

* <span data-ttu-id="15ea2-642">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="15ea2-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="15ea2-643">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="15ea2-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="15ea2-644">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="15ea2-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="15ea2-645">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="15ea2-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-646">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-646">SQL</span></span>

* <span data-ttu-id="15ea2-647">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-648">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-648">VM</span></span>

* <span data-ttu-id="15ea2-649">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="15ea2-650">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="15ea2-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="15ea2-651">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="15ea2-652">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="15ea2-653">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="15ea2-654">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="15ea2-654">August 31, 2017</span></span>

<span data-ttu-id="15ea2-655">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="15ea2-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ea2-656">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15ea2-656">Keyvault</span></span>

* <span data-ttu-id="15ea2-657">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="15ea2-658">Sf</span><span class="sxs-lookup"><span data-stu-id="15ea2-658">Sf</span></span>

* <span data-ttu-id="15ea2-659">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-660">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-660">Storage</span></span>

* <span data-ttu-id="15ea2-661">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="15ea2-662">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="15ea2-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="15ea2-663">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="15ea2-663">August 28, 2017</span></span>

<span data-ttu-id="15ea2-664">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="15ea2-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="15ea2-665">CLI</span><span class="sxs-lookup"><span data-stu-id="15ea2-665">CLI</span></span>

* <span data-ttu-id="15ea2-666">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-667">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-667">ACS</span></span>

* <span data-ttu-id="15ea2-668">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-668">Corrected preview regions</span></span>
* <span data-ttu-id="15ea2-669">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="15ea2-670">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-671">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-671">Appservice</span></span>

* <span data-ttu-id="15ea2-672">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="15ea2-673">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="15ea2-674">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="15ea2-675">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="15ea2-676">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="15ea2-677">IoT</span><span class="sxs-lookup"><span data-stu-id="15ea2-677">IoT</span></span>

* <span data-ttu-id="15ea2-678">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-679">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-679">Network</span></span>

* <span data-ttu-id="15ea2-680">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15ea2-681">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="15ea2-682">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15ea2-683">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15ea2-684">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-685">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-685">Profile</span></span>

* <span data-ttu-id="15ea2-686">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ea2-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ea2-687">Service Fabric</span></span>

* <span data-ttu-id="15ea2-688">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-688">Preview release</span></span>
* <span data-ttu-id="15ea2-689">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="15ea2-690">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="15ea2-691">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-692">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-692">Storage</span></span>

* <span data-ttu-id="15ea2-693">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="15ea2-694">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="15ea2-695">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="15ea2-696">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="15ea2-697">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="15ea2-698">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-699">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-699">VM</span></span>

* <span data-ttu-id="15ea2-700">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="15ea2-701">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="15ea2-702">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ea2-703">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="15ea2-704">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="15ea2-705">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="15ea2-706">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="15ea2-706">August 15, 2017</span></span>

<span data-ttu-id="15ea2-707">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="15ea2-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-708">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-708">ACS</span></span>

* <span data-ttu-id="15ea2-709">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-710">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-710">Appservice</span></span>

* <span data-ttu-id="15ea2-711">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ea2-712">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ea2-712">Event Grid</span></span>

* <span data-ttu-id="15ea2-713">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="15ea2-714">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="15ea2-714">August 11, 2017</span></span>

<span data-ttu-id="15ea2-715">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="15ea2-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-716">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-716">ACS</span></span>

* <span data-ttu-id="15ea2-717">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="15ea2-718">Batch</span><span class="sxs-lookup"><span data-stu-id="15ea2-718">Batch</span></span>

* <span data-ttu-id="15ea2-719">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="15ea2-720">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="15ea2-721">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="15ea2-722">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="15ea2-723">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="15ea2-724">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="15ea2-725">구성 요소</span><span class="sxs-lookup"><span data-stu-id="15ea2-725">Component</span></span>

* <span data-ttu-id="15ea2-726">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="15ea2-727">컨테이너</span><span class="sxs-lookup"><span data-stu-id="15ea2-727">Container</span></span>

* <span data-ttu-id="15ea2-728">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="15ea2-729">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ea2-729">Data Lake Store</span></span>

* <span data-ttu-id="15ea2-730">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ea2-731">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ea2-731">Event Grid</span></span>

* <span data-ttu-id="15ea2-732">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-733">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-733">Network</span></span>

* <span data-ttu-id="15ea2-734">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="15ea2-735">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="15ea2-736">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="15ea2-737">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-738">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-738">Profile</span></span>

* <span data-ttu-id="15ea2-739">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-740">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-740">Storage</span></span>

* <span data-ttu-id="15ea2-741">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-742">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-742">VM</span></span>

* <span data-ttu-id="15ea2-743">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="15ea2-744">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="15ea2-745">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="15ea2-746">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="15ea2-747">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="15ea2-748">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="15ea2-748">July 28, 2017</span></span>

<span data-ttu-id="15ea2-749">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="15ea2-749">Version 2.0.12</span></span>

* <span data-ttu-id="15ea2-750">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-750">Added container commands</span></span>
* <span data-ttu-id="15ea2-751">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-751">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="15ea2-752">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-752">Core</span></span>

* <span data-ttu-id="15ea2-753">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="15ea2-754">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="15ea2-755">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="15ea2-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="15ea2-756">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="15ea2-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="15ea2-757">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="15ea2-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="15ea2-758">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="15ea2-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="15ea2-759">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="15ea2-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15ea2-760">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="15ea2-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="15ea2-761">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="15ea2-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="15ea2-762">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="15ea2-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="15ea2-763">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="15ea2-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="15ea2-764">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="15ea2-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="15ea2-765">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="15ea2-766">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="15ea2-767">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="15ea2-768">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="15ea2-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="15ea2-769">ACR</span><span class="sxs-lookup"><span data-stu-id="15ea2-769">ACR</span></span>

* <span data-ttu-id="15ea2-770">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="15ea2-771">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="15ea2-772">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="15ea2-773">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="15ea2-774">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="15ea2-775">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-776">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-776">ACS</span></span>

* <span data-ttu-id="15ea2-777">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-778">App Service</span><span class="sxs-lookup"><span data-stu-id="15ea2-778">Appservice</span></span>

* <span data-ttu-id="15ea2-779">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="15ea2-780">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="15ea2-781">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="15ea2-782">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="15ea2-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="15ea2-783">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="15ea2-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="15ea2-784">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="15ea2-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="15ea2-785">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="15ea2-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="15ea2-786">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="15ea2-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="15ea2-787">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="15ea2-788">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="15ea2-789">Batch</span><span class="sxs-lookup"><span data-stu-id="15ea2-789">Batch</span></span>

* <span data-ttu-id="15ea2-790">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="15ea2-791">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="15ea2-792">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="15ea2-793">CDN</span><span class="sxs-lookup"><span data-stu-id="15ea2-793">CDN</span></span>

* <span data-ttu-id="15ea2-794">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="15ea2-795">클라우드</span><span class="sxs-lookup"><span data-stu-id="15ea2-795">Cloud</span></span>

* <span data-ttu-id="15ea2-796">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="15ea2-797">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="15ea2-798">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="15ea2-799">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="15ea2-800">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ea2-801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ea2-801">CosmosDB</span></span>

* <span data-ttu-id="15ea2-802">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="15ea2-803">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ea2-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15ea2-804">Data Lake Analytics</span></span>

* <span data-ttu-id="15ea2-805">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="15ea2-806">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="15ea2-807">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ea2-808">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ea2-808">Data Lake Store</span></span>

* <span data-ttu-id="15ea2-809">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="15ea2-810">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="15ea2-811">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="15ea2-812">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="15ea2-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="15ea2-813">대화형</span><span class="sxs-lookup"><span data-stu-id="15ea2-813">Interactive</span></span>

* <span data-ttu-id="15ea2-814">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="15ea2-815">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-815">Increased test coverage</span></span>
* <span data-ttu-id="15ea2-816">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="15ea2-817">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="15ea2-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="15ea2-818">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="15ea2-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="15ea2-819">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="15ea2-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="15ea2-820">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="15ea2-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15ea2-821">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-821">Added `--progress` flag</span></span>
* <span data-ttu-id="15ea2-822">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="15ea2-823">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="15ea2-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="15ea2-824">IoT</span><span class="sxs-lookup"><span data-stu-id="15ea2-824">IoT</span></span>

* <span data-ttu-id="15ea2-825">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="15ea2-826">(#3934)</span><span class="sxs-lookup"><span data-stu-id="15ea2-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ea2-827">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="15ea2-827">Key vault</span></span>

* <span data-ttu-id="15ea2-828">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="15ea2-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="15ea2-829">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ea2-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="15ea2-830">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ea2-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15ea2-831">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ea2-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15ea2-832">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ea2-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="15ea2-833">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="15ea2-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="15ea2-834">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="15ea2-835">(#3307)</span><span class="sxs-lookup"><span data-stu-id="15ea2-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="15ea2-836">랩</span><span class="sxs-lookup"><span data-stu-id="15ea2-836">Lab</span></span>

* <span data-ttu-id="15ea2-837">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="15ea2-838">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-839">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-839">Monitor</span></span>

* <span data-ttu-id="15ea2-840">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="15ea2-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="15ea2-841">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="15ea2-842">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="15ea2-843">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="15ea2-844">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="15ea2-845">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="15ea2-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="15ea2-846">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="15ea2-847">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="15ea2-848">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-848">`location` no longer required</span></span>
  * <span data-ttu-id="15ea2-849">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="15ea2-850">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="15ea2-851">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="15ea2-852">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="15ea2-853">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="15ea2-854">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="15ea2-855">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-856">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-856">Network</span></span>

* <span data-ttu-id="15ea2-857">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="15ea2-858">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="15ea2-859">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="15ea2-860">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="15ea2-861">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="15ea2-862">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="15ea2-863">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="15ea2-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="15ea2-864">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="15ea2-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="15ea2-865">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="15ea2-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="15ea2-866">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15ea2-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="15ea2-867">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15ea2-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="15ea2-868">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="15ea2-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="15ea2-869">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="15ea2-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="15ea2-870">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15ea2-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="15ea2-871">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="15ea2-872">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="15ea2-873">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="15ea2-874">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="15ea2-875">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="15ea2-876">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="15ea2-877">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="15ea2-878">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="15ea2-879">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="15ea2-880">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="15ea2-881">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="15ea2-882">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="15ea2-883">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-884">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-884">Profile</span></span>

* <span data-ttu-id="15ea2-885">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="15ea2-886">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="15ea2-887">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="15ea2-888">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="15ea2-889">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ea2-890">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ea2-890">RDBMS</span></span>

* <span data-ttu-id="15ea2-891">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="15ea2-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="15ea2-892">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="15ea2-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="15ea2-893">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="15ea2-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="15ea2-894">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="15ea2-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-895">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-895">Resource</span></span>

* <span data-ttu-id="15ea2-896">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="15ea2-897">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="15ea2-898">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="15ea2-899">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="15ea2-900">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="15ea2-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="15ea2-901">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="15ea2-902">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="15ea2-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="15ea2-903">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-904">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-904">Role</span></span>

* <span data-ttu-id="15ea2-905">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="15ea2-906">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="15ea2-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="15ea2-907">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="15ea2-908">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="15ea2-909">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ea2-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ea2-910">Service Fabric</span></span>
* <span data-ttu-id="15ea2-911">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="15ea2-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="15ea2-912">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="15ea2-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="15ea2-913">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="15ea2-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-914">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-914">SQL</span></span>

* <span data-ttu-id="15ea2-915">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="15ea2-916">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="15ea2-917">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-918">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-918">Storage</span></span>

* <span data-ttu-id="15ea2-919">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="15ea2-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="15ea2-920">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="15ea2-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="15ea2-921">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="15ea2-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="15ea2-922">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="15ea2-923">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="15ea2-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="15ea2-924">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="15ea2-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-925">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-925">VM</span></span>

* <span data-ttu-id="15ea2-926">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-926">Support configuring nsg</span></span>
* <span data-ttu-id="15ea2-927">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="15ea2-928">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-928">Support managed service identities</span></span>
* <span data-ttu-id="15ea2-929">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="15ea2-930">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="15ea2-931">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="15ea2-931">May 10, 2017</span></span>

<span data-ttu-id="15ea2-932">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="15ea2-932">Version 2.0.6</span></span>

* <span data-ttu-id="15ea2-933">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="15ea2-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="15ea2-934">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="15ea2-935">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="15ea2-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="15ea2-936">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="15ea2-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="15ea2-937">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="15ea2-937">Include Service Fabric module</span></span>
* <span data-ttu-id="15ea2-938">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="15ea2-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="15ea2-939">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-939">Add support for CDN commands</span></span>
* <span data-ttu-id="15ea2-940">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="15ea2-940">Remove Container module</span></span>
* <span data-ttu-id="15ea2-941">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="15ea2-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="15ea2-942">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15ea2-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="15ea2-943">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-943">Core</span></span>

* <span data-ttu-id="15ea2-944">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="15ea2-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="15ea2-945">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="15ea2-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="15ea2-946">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="15ea2-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="15ea2-947">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="15ea2-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="15ea2-948">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="15ea2-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="15ea2-949">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="15ea2-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="15ea2-950">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="15ea2-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="15ea2-951">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="15ea2-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="15ea2-952">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="15ea2-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="15ea2-953">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="15ea2-953">core: Improved performance</span></span>
* <span data-ttu-id="15ea2-954">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="15ea2-955">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="15ea2-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-956">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-956">ACS</span></span>

* <span data-ttu-id="15ea2-957">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="15ea2-958">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="15ea2-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="15ea2-959">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="15ea2-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="15ea2-960">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="15ea2-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-961">AppService</span><span class="sxs-lookup"><span data-stu-id="15ea2-961">AppService</span></span>

* <span data-ttu-id="15ea2-962">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="15ea2-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="15ea2-963">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="15ea2-964">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="15ea2-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="15ea2-965">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="15ea2-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="15ea2-966">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="15ea2-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="15ea2-967">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="15ea2-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="15ea2-968">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-968">support slot swap with preview</span></span>
* <span data-ttu-id="15ea2-969">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="15ea2-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="15ea2-970">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="15ea2-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ea2-971">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ea2-971">CosmosDB</span></span>

* <span data-ttu-id="15ea2-972">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="15ea2-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="15ea2-973">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="15ea2-974">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="15ea2-975">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ea2-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15ea2-976">Data Lake Analytics</span></span>

* <span data-ttu-id="15ea2-977">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="15ea2-978">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="15ea2-979">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="15ea2-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="15ea2-980">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="15ea2-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="15ea2-981">테이블</span><span class="sxs-lookup"><span data-stu-id="15ea2-981">Table</span></span>
  * <span data-ttu-id="15ea2-982">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="15ea2-982">Table valued function</span></span>
  * <span data-ttu-id="15ea2-983">보기</span><span class="sxs-lookup"><span data-stu-id="15ea2-983">View</span></span>
  * <span data-ttu-id="15ea2-984">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="15ea2-984">Table Statistics.</span></span> <span data-ttu-id="15ea2-985">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="15ea2-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ea2-986">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ea2-986">Data Lake Store</span></span>

* <span data-ttu-id="15ea2-987">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="15ea2-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="15ea2-988">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15ea2-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="15ea2-989">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="15ea2-989">missed help for access show.</span></span> <span data-ttu-id="15ea2-990">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-990">adding it.</span></span> <span data-ttu-id="15ea2-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="15ea2-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="15ea2-992">찾기</span><span class="sxs-lookup"><span data-stu-id="15ea2-992">Find</span></span>

* <span data-ttu-id="15ea2-993">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="15ea2-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ea2-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ea2-994">KeyVault</span></span>

* <span data-ttu-id="15ea2-995">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="15ea2-996">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="15ea2-997">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="15ea2-998">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="15ea2-999">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="15ea2-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="15ea2-1000">랩</span><span class="sxs-lookup"><span data-stu-id="15ea2-1000">Lab</span></span>

* <span data-ttu-id="15ea2-1001">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="15ea2-1002">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="15ea2-1003">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="15ea2-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="15ea2-1004">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="15ea2-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="15ea2-1005">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="15ea2-1006">모니터</span><span class="sxs-lookup"><span data-stu-id="15ea2-1006">Monitor</span></span>

* <span data-ttu-id="15ea2-1007">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="15ea2-1008">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="15ea2-1009">네트워크</span><span class="sxs-lookup"><span data-stu-id="15ea2-1009">Network</span></span>

* <span data-ttu-id="15ea2-1010">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="15ea2-1011">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="15ea2-1012">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="15ea2-1013">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="15ea2-1014">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="15ea2-1015">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="15ea2-1016">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="15ea2-1017">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="15ea2-1018">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="15ea2-1019">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="15ea2-1020">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="15ea2-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="15ea2-1021">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="15ea2-1022">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="15ea2-1023">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="15ea2-1024">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="15ea2-1025">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="15ea2-1026">프로필</span><span class="sxs-lookup"><span data-stu-id="15ea2-1026">Profile</span></span>

* <span data-ttu-id="15ea2-1027">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="15ea2-1028">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="15ea2-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="15ea2-1029">Redis</span></span>

* <span data-ttu-id="15ea2-1030">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="15ea2-1031">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="15ea2-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="15ea2-1032">리소스</span><span class="sxs-lookup"><span data-stu-id="15ea2-1032">Resource</span></span>

* <span data-ttu-id="15ea2-1033">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="15ea2-1034">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="15ea2-1035">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="15ea2-1036">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="15ea2-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="15ea2-1038">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1038">Add docs for az lock update.</span></span> <span data-ttu-id="15ea2-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="15ea2-1040">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="15ea2-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="15ea2-1042">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="15ea2-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="15ea2-1044">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="15ea2-1045">역할</span><span class="sxs-lookup"><span data-stu-id="15ea2-1045">Role</span></span>

* <span data-ttu-id="15ea2-1046">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="15ea2-1047">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="15ea2-1048">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="15ea2-1049">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="15ea2-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="15ea2-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="15ea2-1050">SQL</span></span>

* <span data-ttu-id="15ea2-1051">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="15ea2-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="15ea2-1052">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="15ea2-1053">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-1053">Storage</span></span>

* <span data-ttu-id="15ea2-1054">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="15ea2-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="15ea2-1055">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="15ea2-1056">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="15ea2-1057">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="15ea2-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-1058">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-1058">VM</span></span>

* <span data-ttu-id="15ea2-1059">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="15ea2-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="15ea2-1060">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="15ea2-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="15ea2-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="15ea2-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="15ea2-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="15ea2-1063">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="15ea2-1064">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="15ea2-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="15ea2-1065">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="15ea2-1066">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="15ea2-1066">April 3, 2017</span></span>

<span data-ttu-id="15ea2-1067">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="15ea2-1067">Version 2.0.2</span></span>

<span data-ttu-id="15ea2-1068">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```
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

### <a name="core"></a><span data-ttu-id="15ea2-1069">코어</span><span class="sxs-lookup"><span data-stu-id="15ea2-1069">Core</span></span>

* <span data-ttu-id="15ea2-1070">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="15ea2-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="15ea2-1071">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="15ea2-1072">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="15ea2-1073">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15ea2-1074">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="15ea2-1075">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="15ea2-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="15ea2-1077">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="15ea2-1078">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="15ea2-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="15ea2-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="15ea2-1079">ACS</span></span>

* <span data-ttu-id="15ea2-1080">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="15ea2-1081">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="15ea2-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="15ea2-1083">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1083">Add support for windows clusters.</span></span> <span data-ttu-id="15ea2-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="15ea2-1085">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="15ea2-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="15ea2-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="15ea2-1087">AppService</span></span>

* <span data-ttu-id="15ea2-1088">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="15ea2-1089">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="15ea2-1090">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="15ea2-1091">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="15ea2-1092">DataLake</span><span class="sxs-lookup"><span data-stu-id="15ea2-1092">DataLake</span></span>

* <span data-ttu-id="15ea2-1093">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="15ea2-1094">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="15ea2-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="15ea2-1095">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="15ea2-1095">DocuemntDB</span></span>

* <span data-ttu-id="15ea2-1096">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="15ea2-1097">VM</span><span class="sxs-lookup"><span data-stu-id="15ea2-1097">VM</span></span>

* <span data-ttu-id="15ea2-1098">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="15ea2-1099">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="15ea2-1100">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="15ea2-1101">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15ea2-1102">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="15ea2-1103">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="15ea2-1104">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="15ea2-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="15ea2-1105">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="15ea2-1105">February 27, 2017</span></span>

<span data-ttu-id="15ea2-1106">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="15ea2-1106">Version 2.0.0</span></span>

<span data-ttu-id="15ea2-1107">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="15ea2-1108">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="15ea2-1108">Container Service (acs)</span></span>
- <span data-ttu-id="15ea2-1109">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="15ea2-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="15ea2-1110">네트워킹</span><span class="sxs-lookup"><span data-stu-id="15ea2-1110">Networking</span></span>
- <span data-ttu-id="15ea2-1111">Storage</span><span class="sxs-lookup"><span data-stu-id="15ea2-1111">Storage</span></span>

<span data-ttu-id="15ea2-1112">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="15ea2-1113">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="15ea2-1114">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```
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
> <span data-ttu-id="15ea2-1115">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="15ea2-1116">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="15ea2-1117">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15ea2-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="15ea2-1118">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="15ea2-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="15ea2-1119">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="15ea2-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="15ea2-1120">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="15ea2-1120">Provide feedback from the command line with the `az feedback` command</span></span>


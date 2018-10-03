---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/21/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f0ee84c3f70cf168818de447289d6c7ab5a40c9e
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178085"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="e7e73-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="e7e73-103">Azure CLI release notes</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="e7e73-104">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="e7e73-104">September 21, 2018</span></span>

<span data-ttu-id="e7e73-105">버전 20.46</span><span class="sxs-lookup"><span data-stu-id="e7e73-105">Version 20.46</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-106">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-106">ACR</span></span>
* <span data-ttu-id="e7e73-107">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-107">Added ACR Task commands</span></span>
* <span data-ttu-id="e7e73-108">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-108">Added quick run command</span></span>
* <span data-ttu-id="e7e73-109">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-109">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="e7e73-110">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-110">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="e7e73-111">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-111">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="e7e73-112">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-112">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-113">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-113">ACS</span></span>
* <span data-ttu-id="e7e73-114">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-114">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="e7e73-115">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-115">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-116">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-116">AppService</span></span>

* <span data-ttu-id="e7e73-117">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-117">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="e7e73-118">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-118">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="e7e73-119">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-119">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="e7e73-120">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-120">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-121">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-121">Batch</span></span>
* <span data-ttu-id="e7e73-122">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-122">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="e7e73-123">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-123">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="e7e73-124">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-124">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="e7e73-125">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-125">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e7e73-126">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e7e73-126">Batch AI</span></span> 
* <span data-ttu-id="e7e73-127">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-127">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e7e73-128">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e7e73-128">Cognitive Services</span></span>
* <span data-ttu-id="e7e73-129">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-129">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="e7e73-130">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-130">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="e7e73-131">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-131">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="e7e73-132">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-132">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="e7e73-133">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-133">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="e7e73-134">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-134">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-135">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-135">Container</span></span>
* <span data-ttu-id="e7e73-136">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-136">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="e7e73-137">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-137">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="e7e73-138">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-138">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="e7e73-139">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-139">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="e7e73-140">Datalake</span><span class="sxs-lookup"><span data-stu-id="e7e73-140">Datalake</span></span>
* <span data-ttu-id="e7e73-141">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-141">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="e7e73-142">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="e7e73-142">Interactive Shell</span></span>
* <span data-ttu-id="e7e73-143">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-143">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="e7e73-144">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-144">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-145">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-145">IoT</span></span>
* <span data-ttu-id="e7e73-146">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-146">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="e7e73-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e7e73-147">Key Vault</span></span>
* <span data-ttu-id="e7e73-148">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-148">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-149">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-149">Network</span></span>
* <span data-ttu-id="e7e73-150">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-150">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="e7e73-151">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-151">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="e7e73-152">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-152">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="e7e73-153">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-153">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="e7e73-154">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-154">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="e7e73-155">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-155">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="e7e73-156">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-156">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="e7e73-157">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-157">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="e7e73-158">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-158">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="e7e73-159">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-159">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="e7e73-160">`network vnet subnet create/update`: `--delegation` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-160">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="e7e73-161">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-161">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="e7e73-162">`network traffic-manager profile create/update`: 모니터 구성을 위한 `--interval`, `--timeout` 및 `--max-failures` 지원 추가. `--path`, `--port`, `--protocol`로 인해 `--monitor-path`, `--monitor-port` 및 `--monitor-protocol` 옵션이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-162">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="e7e73-163">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하기 위한 논리 수정. 사설 IP 주소가 제공된 경우 할당이 정적이 됨. 사설 IP 주소가 제공되지 않은 경우 사설 IP 주소에 대해 빈 문자열이 제공되고 할당이 동적이 됨.</span><span class="sxs-lookup"><span data-stu-id="e7e73-163">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="e7e73-164">`dns record-set * create/update`: `--target-resource` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-164">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="e7e73-165">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-165">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="e7e73-166">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-166">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="e7e73-167">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-167">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-168">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-168">RDBMS</span></span>
* <span data-ttu-id="e7e73-169">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-169">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="e7e73-170">예약</span><span class="sxs-lookup"><span data-stu-id="e7e73-170">Reservation</span></span>
* <span data-ttu-id="e7e73-171">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-171">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="e7e73-172">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-172">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="e7e73-173">앱 관리</span><span class="sxs-lookup"><span data-stu-id="e7e73-173">Manage App</span></span>
* <span data-ttu-id="e7e73-174">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-174">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="e7e73-175">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-175">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-176">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-176">Role</span></span>
* <span data-ttu-id="e7e73-177">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-177">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="e7e73-178">SignalR</span><span class="sxs-lookup"><span data-stu-id="e7e73-178">SignalR</span></span>
* <span data-ttu-id="e7e73-179">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-179">First release</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-180">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-180">Storage</span></span>
* <span data-ttu-id="e7e73-181">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-181">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="e7e73-182">변경할 수 없는 저장소 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-182">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-183">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-183">VM</span></span>
* <span data-ttu-id="e7e73-184">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="e7e73-184">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="e7e73-185">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-185">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="e7e73-186">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="e7e73-186">August 28, 2018</span></span>

<span data-ttu-id="e7e73-187">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="e7e73-187">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-188">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-188">Core</span></span>

* <span data-ttu-id="e7e73-189">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-189">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="e7e73-190">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-190">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-191">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-191">ACR</span></span>

* <span data-ttu-id="e7e73-192">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-192">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="e7e73-193">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-193">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-194">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-194">ACS</span></span>

* <span data-ttu-id="e7e73-195">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-195">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="e7e73-196">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-196">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-197">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-197">AppService</span></span>

* <span data-ttu-id="e7e73-198">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-198">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="e7e73-199">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-199">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="e7e73-200">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-200">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="e7e73-201">Backup</span><span class="sxs-lookup"><span data-stu-id="e7e73-201">Backup</span></span>

* <span data-ttu-id="e7e73-202">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-202">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="e7e73-203">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="e7e73-203">Bot Service</span></span>

* <span data-ttu-id="e7e73-204">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-204">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e7e73-205">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e7e73-205">Cognitive Services</span></span>

* <span data-ttu-id="e7e73-206">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-206">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-207">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-207">IoT</span></span>

* <span data-ttu-id="e7e73-208">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-208">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-209">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-209">Monitor</span></span>

* <span data-ttu-id="e7e73-210">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-210">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="e7e73-211">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="e7e73-211">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-212">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-212">Network</span></span>

* <span data-ttu-id="e7e73-213">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-213">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-214">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-214">Resource</span></span>

* <span data-ttu-id="e7e73-215">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-215">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-216">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-216">Storage</span></span>

* <span data-ttu-id="e7e73-217">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-217">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-218">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-218">VM</span></span>

* <span data-ttu-id="e7e73-219">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-219">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="e7e73-220">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="e7e73-220">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="e7e73-221">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="e7e73-221">Auguest 14, 2018</span></span>

<span data-ttu-id="e7e73-222">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="e7e73-222">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-223">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-223">Core</span></span>

* <span data-ttu-id="e7e73-224">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-224">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="e7e73-225">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="e7e73-225">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="e7e73-226">원격 분석</span><span class="sxs-lookup"><span data-stu-id="e7e73-226">Telemetry</span></span>

* <span data-ttu-id="e7e73-227">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="e7e73-227">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-228">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-228">ACR</span></span>

* <span data-ttu-id="e7e73-229">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-229">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="e7e73-230">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-230">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-231">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-231">ACS</span></span>

* <span data-ttu-id="e7e73-232">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-232">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="e7e73-233">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-233">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="e7e73-234">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-234">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="e7e73-235">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-235">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="e7e73-236">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-236">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="e7e73-237">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-237">AppService</span></span>

* <span data-ttu-id="e7e73-238">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-238">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="e7e73-239">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-239">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="e7e73-240">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e7e73-240">BatchAI</span></span>

* <span data-ttu-id="e7e73-241">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-241">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="e7e73-242">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-242">Container</span></span>

* <span data-ttu-id="e7e73-243">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-243">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="e7e73-244">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-244">IoT</span></span>

* <span data-ttu-id="e7e73-245">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="e7e73-245">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="e7e73-246">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-246">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="e7e73-247">Iot Central</span><span class="sxs-lookup"><span data-stu-id="e7e73-247">Iot Central</span></span>

* <span data-ttu-id="e7e73-248">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-248">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-249">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e7e73-249">KeyVault</span></span>


* <span data-ttu-id="e7e73-250">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-250">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="e7e73-251">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-251">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="e7e73-252">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-252">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="e7e73-253">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-253">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="e7e73-254">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-254">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="e7e73-255">릴레이</span><span class="sxs-lookup"><span data-stu-id="e7e73-255">Relay</span></span>

* <span data-ttu-id="e7e73-256">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-256">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-257">Sql</span><span class="sxs-lookup"><span data-stu-id="e7e73-257">Sql</span></span>

* <span data-ttu-id="e7e73-258">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-258">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-259">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-259">Storage</span></span>

* <span data-ttu-id="e7e73-260">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-260">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="e7e73-261">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-261">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="e7e73-262">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-262">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="e7e73-263">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="e7e73-263">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="e7e73-264">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-264">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-265">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-265">VM</span></span>

* <span data-ttu-id="e7e73-266">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-266">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e7e73-267">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="e7e73-267">July 31, 2018</span></span>

<span data-ttu-id="e7e73-268">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e7e73-268">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-269">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-269">ACR</span></span>

* <span data-ttu-id="e7e73-270">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-270">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e7e73-271">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-271">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-272">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-272">ACS</span></span>

* <span data-ttu-id="e7e73-273">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-273">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-274">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-274">Batch</span></span>

* <span data-ttu-id="e7e73-275">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-275">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-276">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-276">Container</span></span>

* <span data-ttu-id="e7e73-277">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-277">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-278">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-278">Network</span></span>

* <span data-ttu-id="e7e73-279">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-279">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e7e73-280">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-280">Resource</span></span>

* <span data-ttu-id="e7e73-281">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="e7e73-281">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e7e73-282">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-282">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-283">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-283">Role</span></span>

* <span data-ttu-id="e7e73-284">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-284">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e7e73-285">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-285">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e7e73-286">검색</span><span class="sxs-lookup"><span data-stu-id="e7e73-286">Search</span></span>

* <span data-ttu-id="e7e73-287">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-287">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e7e73-288">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e7e73-288">Service Bus</span></span>

* <span data-ttu-id="e7e73-289">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-289">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e7e73-290">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-290">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e7e73-291">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="e7e73-291">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e7e73-292">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="e7e73-292">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-293">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-293">Storage</span></span>

* <span data-ttu-id="e7e73-294">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-294">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e7e73-295">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="e7e73-295">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-296">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-296">VM</span></span>

* <span data-ttu-id="e7e73-297">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-297">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e7e73-298">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-298">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e7e73-299">VM 확장 집합 생성 시 응용 프로그램 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-299">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e7e73-300">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-300">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e7e73-301">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="e7e73-301">July 18, 2018</span></span>

<span data-ttu-id="e7e73-302">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e7e73-302">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-303">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-303">Core</span></span>

* <span data-ttu-id="e7e73-304">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-304">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e7e73-305">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-305">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e7e73-306">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-306">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-307">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-307">ACR</span></span>

* <span data-ttu-id="e7e73-308">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-308">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e7e73-309">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-309">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e7e73-310">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-310">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e7e73-311">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-311">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-312">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-312">ACS</span></span>

* <span data-ttu-id="e7e73-313">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-313">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-314">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-314">AppService</span></span>

* <span data-ttu-id="e7e73-315">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-315">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-316">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-316">Batch</span></span>

* <span data-ttu-id="e7e73-317">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-317">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e7e73-318">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-318">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e7e73-319">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e7e73-319">Batch AI</span></span>

* <span data-ttu-id="e7e73-320">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-320">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-321">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-321">Container</span></span>

* <span data-ttu-id="e7e73-322">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-322">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e7e73-323">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-323">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-324">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-324">Network</span></span>

* <span data-ttu-id="e7e73-325">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-325">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e7e73-326">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-326">Added `network nic wait`</span></span>
* <span data-ttu-id="e7e73-327">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-327">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e7e73-328">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-328">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e7e73-329">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-329">Resource</span></span>

* <span data-ttu-id="e7e73-330">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-330">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e7e73-331">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-331">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e7e73-332">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-332">Added `deployment wait` command</span></span>
* <span data-ttu-id="e7e73-333">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-333">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-334">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-334">SQL</span></span>

* <span data-ttu-id="e7e73-335">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-335">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e7e73-336">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-336">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e7e73-337">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="e7e73-337">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-338">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-338">Storage</span></span>

* <span data-ttu-id="e7e73-339">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-339">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-340">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-340">VM</span></span>

* <span data-ttu-id="e7e73-341">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-341">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e7e73-342">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-342">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e7e73-343">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-343">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e7e73-344">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="e7e73-344">July 3, 2018</span></span>

<span data-ttu-id="e7e73-345">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e7e73-345">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e7e73-346">AKS</span><span class="sxs-lookup"><span data-stu-id="e7e73-346">AKS</span></span>

* <span data-ttu-id="e7e73-347">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-347">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e7e73-348">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="e7e73-348">July 3, 2018</span></span>

<span data-ttu-id="e7e73-349">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e7e73-349">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-350">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-350">Core</span></span>

* <span data-ttu-id="e7e73-351">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-351">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-352">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-352">ACR</span></span>

* <span data-ttu-id="e7e73-353">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-353">Added polling build status</span></span>
* <span data-ttu-id="e7e73-354">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-354">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e7e73-355">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-355">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-356">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-356">ACS</span></span>

* <span data-ttu-id="e7e73-357">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-357">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e7e73-358">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-358">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e7e73-359">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="e7e73-359">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e7e73-360">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-360">Added `--listen-port` support</span></span>
* <span data-ttu-id="e7e73-361">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="e7e73-361">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e7e73-362">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="e7e73-362">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e7e73-363">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-363">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-364">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-364">AppService</span></span>

* <span data-ttu-id="e7e73-365">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-365">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e7e73-366">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-366">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e7e73-367">Backup</span><span class="sxs-lookup"><span data-stu-id="e7e73-367">Backup</span></span>

* <span data-ttu-id="e7e73-368">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-368">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e7e73-369">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e7e73-369">BatchAI</span></span>

* <span data-ttu-id="e7e73-370">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-370">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e7e73-371">클라우드</span><span class="sxs-lookup"><span data-stu-id="e7e73-371">Cloud</span></span>

* <span data-ttu-id="e7e73-372">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-372">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-373">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-373">Container</span></span>

* <span data-ttu-id="e7e73-374">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-374">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e7e73-375">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-375">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e7e73-376">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-376">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-377">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-377">Extension</span></span>

* <span data-ttu-id="e7e73-378">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-378">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-379">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-379">Network</span></span>

* <span data-ttu-id="e7e73-380">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e7e73-380">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-381">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e7e73-381">Rdbms</span></span>

* <span data-ttu-id="e7e73-382">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-382">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-383">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-383">Resource</span></span>

* <span data-ttu-id="e7e73-384">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-384">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-385">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-385">VM</span></span>

* <span data-ttu-id="e7e73-386">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-386">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e7e73-387">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="e7e73-387">June 25, 2018</span></span>

<span data-ttu-id="e7e73-388">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e7e73-388">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e7e73-389">CLI</span><span class="sxs-lookup"><span data-stu-id="e7e73-389">CLI</span></span>

* <span data-ttu-id="e7e73-390">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-390">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e7e73-391">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="e7e73-391">June 19, 2018</span></span>

<span data-ttu-id="e7e73-392">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e7e73-392">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-393">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-393">Core</span></span>

* <span data-ttu-id="e7e73-394">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-394">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-395">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-395">ACR</span></span>

* <span data-ttu-id="e7e73-396">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-396">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e7e73-397">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-397">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-398">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-398">ACS</span></span>

* <span data-ttu-id="e7e73-399">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="e7e73-399">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e7e73-400">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-400">Added `--update` support</span></span>
* <span data-ttu-id="e7e73-401">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-401">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e7e73-402">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="e7e73-402">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e7e73-403">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-403">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e7e73-404">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-404">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e7e73-405">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-405">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e7e73-406">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-406">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-407">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-407">AppService</span></span>

* <span data-ttu-id="e7e73-408">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-408">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e7e73-409">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-409">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-410">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-410">Batch</span></span>

* <span data-ttu-id="e7e73-411">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-411">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e7e73-412">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e7e73-412">Batch AI</span></span>

* <span data-ttu-id="e7e73-413">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="e7e73-413">Added support for workspaces.</span></span> <span data-ttu-id="e7e73-414">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-414">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e7e73-415">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="e7e73-415">Added support for experiments.</span></span> <span data-ttu-id="e7e73-416">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-416">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e7e73-417">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-417">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e7e73-418">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="e7e73-418">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e7e73-419">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-419">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e7e73-420">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-420">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e7e73-421">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="e7e73-421">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e7e73-422">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="e7e73-422">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e7e73-423">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="e7e73-423">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e7e73-424">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="e7e73-424">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e7e73-425">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="e7e73-425">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e7e73-426">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="e7e73-426">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e7e73-427">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="e7e73-427">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e7e73-428">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-428">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e7e73-429">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-429">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e7e73-430">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="e7e73-430">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="e7e73-431">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="e7e73-431">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="e7e73-432">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="e7e73-432">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e7e73-433">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="e7e73-433">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e7e73-434">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="e7e73-434">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e7e73-435">지도</span><span class="sxs-lookup"><span data-stu-id="e7e73-435">Maps</span></span>

* <span data-ttu-id="e7e73-436">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-436">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-437">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-437">Network</span></span>

* <span data-ttu-id="e7e73-438">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-438">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e7e73-439">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-439">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e7e73-440">#6502</span><span class="sxs-lookup"><span data-stu-id="e7e73-440">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e7e73-441">예약</span><span class="sxs-lookup"><span data-stu-id="e7e73-441">Reservations</span></span>

* <span data-ttu-id="e7e73-442">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-442">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e7e73-443">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-443">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e7e73-444">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-444">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e7e73-445">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-445">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e7e73-446">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-446">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e7e73-447">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-447">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-448">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-448">Role</span></span>

* <span data-ttu-id="e7e73-449">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="e7e73-449">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-450">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-450">SQL</span></span>

* <span data-ttu-id="e7e73-451">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-451">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-452">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-452">Storage</span></span>

* <span data-ttu-id="e7e73-453">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="e7e73-453">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-454">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-454">VM</span></span>

* <span data-ttu-id="e7e73-455">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="e7e73-455">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e7e73-456">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-456">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e7e73-457">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-457">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e7e73-458">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="e7e73-458">June 13, 2018</span></span>

<span data-ttu-id="e7e73-459">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e7e73-459">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-460">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-460">Core</span></span>

* <span data-ttu-id="e7e73-461">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="e7e73-461">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e7e73-462">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="e7e73-462">June 13, 2018</span></span>

<span data-ttu-id="e7e73-463">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e7e73-463">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e7e73-464">AKS</span><span class="sxs-lookup"><span data-stu-id="e7e73-464">AKS</span></span>

* <span data-ttu-id="e7e73-465">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-465">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e7e73-466">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="e7e73-466">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e7e73-467">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-467">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e7e73-468">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-468">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e7e73-469">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-469">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-470">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-470">AppService</span></span>

* <span data-ttu-id="e7e73-471">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-471">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e7e73-472">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="e7e73-472">June 5, 2018</span></span>

<span data-ttu-id="e7e73-473">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e7e73-473">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-474">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-474">Interactive</span></span>

* <span data-ttu-id="e7e73-475">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="e7e73-475">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e7e73-476">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="e7e73-476">June 5, 2018</span></span>

<span data-ttu-id="e7e73-477">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e7e73-477">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-478">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-478">Core</span></span>

* <span data-ttu-id="e7e73-479">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-479">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e7e73-480">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-480">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-481">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-481">ACR</span></span>

* <span data-ttu-id="e7e73-482">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-482">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e7e73-483">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-483">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e7e73-484">AKS</span><span class="sxs-lookup"><span data-stu-id="e7e73-484">AKS</span></span>

* <span data-ttu-id="e7e73-485">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-485">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-486">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-486">Batch</span></span>

* <span data-ttu-id="e7e73-487">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e7e73-487">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-488">IOT</span><span class="sxs-lookup"><span data-stu-id="e7e73-488">IOT</span></span>

* <span data-ttu-id="e7e73-489">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-489">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-490">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-490">Network</span></span>

* <span data-ttu-id="e7e73-491">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="e7e73-491">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e7e73-492">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e7e73-492">Policy Insights</span></span>

* <span data-ttu-id="e7e73-493">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-493">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e7e73-494">ARM</span><span class="sxs-lookup"><span data-stu-id="e7e73-494">ARM</span></span>

* <span data-ttu-id="e7e73-495">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-495">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-496">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-496">SQL</span></span>

* <span data-ttu-id="e7e73-497">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="e7e73-497">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e7e73-498">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-498">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e7e73-499">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-499">Storage</span></span>

* <span data-ttu-id="e7e73-500">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="e7e73-500">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-501">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-501">VM</span></span>

* <span data-ttu-id="e7e73-502">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-502">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e7e73-503">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-503">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e7e73-504">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-504">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e7e73-505">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="e7e73-505">May 22, 2018</span></span>

<span data-ttu-id="e7e73-506">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e7e73-506">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-507">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-507">Core</span></span>

* <span data-ttu-id="e7e73-508">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-508">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-509">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-509">ACS</span></span>

* <span data-ttu-id="e7e73-510">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-510">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e7e73-511">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-511">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-512">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-512">AppService</span></span>

* <span data-ttu-id="e7e73-513">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-513">Improved generic update commands</span></span>
* <span data-ttu-id="e7e73-514">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-514">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-515">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-515">Container</span></span>

* <span data-ttu-id="e7e73-516">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-516">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e7e73-517">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-517">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-518">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-518">Extension</span></span>

* <span data-ttu-id="e7e73-519">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-519">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-520">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-520">Interactive</span></span>

* <span data-ttu-id="e7e73-521">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-521">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e7e73-522">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="e7e73-522">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-523">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e7e73-523">KeyVault</span></span>

* <span data-ttu-id="e7e73-524">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="e7e73-524">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-525">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-525">Network</span></span>

* <span data-ttu-id="e7e73-526">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="e7e73-526">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e7e73-527">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-527">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-528">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-528">SQL</span></span>

* <span data-ttu-id="e7e73-529">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="e7e73-529">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e7e73-530">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="e7e73-530">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e7e73-531">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-531">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e7e73-532">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-532">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e7e73-533">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-533">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e7e73-534">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e7e73-534">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e7e73-535">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-535">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e7e73-536">`edition`</span><span class="sxs-lookup"><span data-stu-id="e7e73-536">`edition`.</span></span> <span data-ttu-id="e7e73-537">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-537">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e7e73-538">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="e7e73-538">`elasticPoolName`.</span></span> <span data-ttu-id="e7e73-539">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-539">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e7e73-540">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-540">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e7e73-541">`edition`</span><span class="sxs-lookup"><span data-stu-id="e7e73-541">`edition`.</span></span> <span data-ttu-id="e7e73-542">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="e7e73-542">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e7e73-543">`dtu`</span><span class="sxs-lookup"><span data-stu-id="e7e73-543">`dtu`.</span></span> <span data-ttu-id="e7e73-544">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="e7e73-544">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e7e73-545">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="e7e73-545">`databaseDtuMin`.</span></span> <span data-ttu-id="e7e73-546">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="e7e73-546">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e7e73-547">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="e7e73-547">`databaseDtuMax`.</span></span> <span data-ttu-id="e7e73-548">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="e7e73-548">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e7e73-549">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-549">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e7e73-550">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-550">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-551">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-551">Storage</span></span>

* <span data-ttu-id="e7e73-552">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-552">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e7e73-553">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-553">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-554">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-554">VM</span></span>

* <span data-ttu-id="e7e73-555">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="e7e73-555">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e7e73-556">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="e7e73-556">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e7e73-557">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="e7e73-557">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e7e73-558">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="e7e73-558">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e7e73-559">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-559">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e7e73-560">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="e7e73-560">May 7, 2018</span></span>

<span data-ttu-id="e7e73-561">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e7e73-561">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-562">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-562">Core</span></span>

* <span data-ttu-id="e7e73-563">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-563">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e7e73-564">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-564">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e7e73-565">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-565">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e7e73-566">#5591</span><span class="sxs-lookup"><span data-stu-id="e7e73-566">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e7e73-567">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-567">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e7e73-568">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-568">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e7e73-569">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-569">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e7e73-570">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-570">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e7e73-571">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-571">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-572">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-572">ACR</span></span>

* <span data-ttu-id="e7e73-573">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-573">Added ACR Build commands</span></span>
* <span data-ttu-id="e7e73-574">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-574">Improved resource not found error messages</span></span>
* <span data-ttu-id="e7e73-575">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-575">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e7e73-576">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-576">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e7e73-577">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-577">Improved repository commands error messages</span></span>
* <span data-ttu-id="e7e73-578">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-578">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-579">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-579">ACS</span></span>

* <span data-ttu-id="e7e73-580">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-580">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e7e73-581">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-581">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e7e73-582">AMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-582">AMS</span></span>

* <span data-ttu-id="e7e73-583">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="e7e73-583">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-584">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-584">Appservice</span></span>

* <span data-ttu-id="e7e73-585">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-585">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e7e73-586">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-586">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e7e73-587">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-587">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e7e73-588">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-588">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e7e73-589">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e7e73-589">Batch AI</span></span>

* <span data-ttu-id="e7e73-590">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-590">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e7e73-591">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e7e73-591">Cognitive Services</span></span>

* <span data-ttu-id="e7e73-592">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-592">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e7e73-593">Consumption</span><span class="sxs-lookup"><span data-stu-id="e7e73-593">Consumption</span></span>

* <span data-ttu-id="e7e73-594">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-594">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-595">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-595">Container</span></span>

* <span data-ttu-id="e7e73-596">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-596">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e7e73-597">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e7e73-597">Cosmos DB</span></span>

* <span data-ttu-id="e7e73-598">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e7e73-598">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e7e73-599">DMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-599">DMS</span></span>

* <span data-ttu-id="e7e73-600">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-600">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-601">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-601">Extension</span></span>

* <span data-ttu-id="e7e73-602">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-602">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-603">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-603">Interactive</span></span>

* <span data-ttu-id="e7e73-604">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-604">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e7e73-605">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="e7e73-605">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e7e73-606">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-606">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e7e73-607">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-607">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e7e73-608">랩</span><span class="sxs-lookup"><span data-stu-id="e7e73-608">Lab</span></span>

* <span data-ttu-id="e7e73-609">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-609">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-610">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-610">Network</span></span>

* <span data-ttu-id="e7e73-611">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-611">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e7e73-612">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-612">Profile</span></span>

* <span data-ttu-id="e7e73-613">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-613">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e7e73-614">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-614">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e7e73-615">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-615">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e7e73-616">Redis</span><span class="sxs-lookup"><span data-stu-id="e7e73-616">Redis</span></span>

* <span data-ttu-id="e7e73-617">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-617">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e7e73-618">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-618">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e7e73-619">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-619">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e7e73-620">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-620">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e7e73-621">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-621">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-622">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-622">Role</span></span>

* <span data-ttu-id="e7e73-623">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-623">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-624">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-624">Storage</span></span>

* <span data-ttu-id="e7e73-625">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-625">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e7e73-626">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="e7e73-626">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e7e73-627">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="e7e73-627">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e7e73-628">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-628">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e7e73-629">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-629">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-630">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-630">VM</span></span>

* <span data-ttu-id="e7e73-631">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-631">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e7e73-632">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-632">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e7e73-633">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="e7e73-633">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e7e73-634">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-634">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e7e73-635">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-635">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e7e73-636">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-636">Added write accelerator support</span></span>
* <span data-ttu-id="e7e73-637">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-637">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e7e73-638">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-638">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e7e73-639">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-639">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e7e73-640">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="e7e73-640">April 10, 2018</span></span>

<span data-ttu-id="e7e73-641">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e7e73-641">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-642">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-642">ACR</span></span>

* <span data-ttu-id="e7e73-643">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="e7e73-643">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-644">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-644">ACS</span></span>

* <span data-ttu-id="e7e73-645">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-645">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-646">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-646">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e7e73-648">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-648">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e7e73-649">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e7e73-649">BatchAI</span></span>

* <span data-ttu-id="e7e73-650">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-650">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="e7e73-651">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="e7e73-651">Job level mounting</span></span>
 - <span data-ttu-id="e7e73-652">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="e7e73-652">Environment variables with secret values</span></span>
 - <span data-ttu-id="e7e73-653">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-653">Performance counters settings</span></span>
 - <span data-ttu-id="e7e73-654">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="e7e73-654">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="e7e73-655">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-655">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="e7e73-656">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="e7e73-656">Usage and limits reporting</span></span>
 - <span data-ttu-id="e7e73-657">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-657">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="e7e73-658">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-658">Support for custom images</span></span>
 - <span data-ttu-id="e7e73-659">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-659">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e7e73-660">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-660">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e7e73-661">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-661">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e7e73-662">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-662">National clouds are supported</span></span>
* <span data-ttu-id="e7e73-663">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-663">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e7e73-664">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="e7e73-664">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e7e73-665">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-665">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e7e73-666">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-666">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e7e73-667">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="e7e73-667">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e7e73-668">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="e7e73-668">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e7e73-669">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-669">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e7e73-670">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-670">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e7e73-671">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-671">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e7e73-672">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-672">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e7e73-673">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-673">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e7e73-674">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="e7e73-674">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e7e73-675">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-675">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e7e73-676">결제</span><span class="sxs-lookup"><span data-stu-id="e7e73-676">Billing</span></span>

* <span data-ttu-id="e7e73-677">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-677">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e7e73-678">Consumption</span><span class="sxs-lookup"><span data-stu-id="e7e73-678">Consumption</span></span>

* <span data-ttu-id="e7e73-679">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-679">Added `marketplace` commands</span></span>
* <span data-ttu-id="e7e73-680">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-680">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e7e73-681">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-681">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e7e73-682">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-682">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e7e73-683">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-683">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e7e73-684">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-684">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-685">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-685">Container</span></span>

* <span data-ttu-id="e7e73-686">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="e7e73-686">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e7e73-687">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="e7e73-687">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-688">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-688">Extension</span></span>

* <span data-ttu-id="e7e73-689">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-689">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-690">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-690">Interactive</span></span>

* <span data-ttu-id="e7e73-691">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-691">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e7e73-692">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-692">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e7e73-693">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-693">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-694">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-694">Network</span></span>

* <span data-ttu-id="e7e73-695">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-695">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e7e73-696">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-696">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e7e73-697">#4910</span><span class="sxs-lookup"><span data-stu-id="e7e73-697">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e7e73-698">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-698">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e7e73-699">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="e7e73-699">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e7e73-700">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-700">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e7e73-701">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-701">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e7e73-702">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-702">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-703">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-703">Profile</span></span>

* <span data-ttu-id="e7e73-704">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-704">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e7e73-705">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-705">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-706">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-706">RDBMS</span></span>

* <span data-ttu-id="e7e73-707">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-707">Added `georestore` command</span></span>
* <span data-ttu-id="e7e73-708">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-708">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-709">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-709">Resource</span></span>

* <span data-ttu-id="e7e73-710">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-710">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e7e73-711">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-711">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-712">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-712">SQL</span></span>

* <span data-ttu-id="e7e73-713">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-713">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-714">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-714">Storage</span></span>

* <span data-ttu-id="e7e73-715">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-715">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-716">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-716">VM</span></span>

* <span data-ttu-id="e7e73-717">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-717">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e7e73-718">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-718">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e7e73-720">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-720">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e7e73-721">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-721">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e7e73-722">#5718</span><span class="sxs-lookup"><span data-stu-id="e7e73-722">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e7e73-723">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-723">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e7e73-724">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="e7e73-724">March 27, 2018</span></span>

<span data-ttu-id="e7e73-725">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e7e73-725">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-726">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-726">Core</span></span>

* <span data-ttu-id="e7e73-727">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="e7e73-727">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-728">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-728">ACS</span></span>

* <span data-ttu-id="e7e73-729">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-729">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-730">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-730">Appservice</span></span>

* <span data-ttu-id="e7e73-731">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-731">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e7e73-732">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-732">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e7e73-733">Backup</span><span class="sxs-lookup"><span data-stu-id="e7e73-733">Backup</span></span>

* <span data-ttu-id="e7e73-734">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-734">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e7e73-735">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-735">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e7e73-736">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-736">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e7e73-737">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-737">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-738">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-738">Container</span></span>

* <span data-ttu-id="e7e73-739">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-739">Added `container exec` command.</span></span> <span data-ttu-id="e7e73-740">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-740">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e7e73-741">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-741">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-742">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-742">Extension</span></span>

* <span data-ttu-id="e7e73-743">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-743">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e7e73-744">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-744">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e7e73-745">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-745">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-746">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-746">Interactive</span></span>

* <span data-ttu-id="e7e73-747">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="e7e73-747">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e7e73-748">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-748">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e7e73-749">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-749">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e7e73-750">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-750">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e7e73-751">랩</span><span class="sxs-lookup"><span data-stu-id="e7e73-751">Lab</span></span>

* <span data-ttu-id="e7e73-752">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-752">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-753">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-753">Monitor</span></span>

* <span data-ttu-id="e7e73-754">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-754">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e7e73-755">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="e7e73-755">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e7e73-756">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-756">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-757">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-757">Network</span></span>

* <span data-ttu-id="e7e73-758">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-758">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-759">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-759">Profile</span></span>

* <span data-ttu-id="e7e73-760">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-760">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-761">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-761">RDBMS</span></span>

* <span data-ttu-id="e7e73-762">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-762">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-763">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-763">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e7e73-765">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-765">Role</span></span>

* <span data-ttu-id="e7e73-766">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-766">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e7e73-767">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-767">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e7e73-768">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-768">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e7e73-769">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-769">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e7e73-770">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-770">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-771">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-771">Storage</span></span>

* <span data-ttu-id="e7e73-772">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-772">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e7e73-773">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="e7e73-773">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-774">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-774">VM</span></span>

* <span data-ttu-id="e7e73-775">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-775">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e7e73-776">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-776">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e7e73-777">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-777">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e7e73-778">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-778">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e7e73-779">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="e7e73-779">March 13, 2018</span></span>

<span data-ttu-id="e7e73-780">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e7e73-780">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-781">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-781">ACR</span></span>

* <span data-ttu-id="e7e73-782">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-782">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e7e73-783">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-783">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e7e73-784">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-784">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-785">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-785">ACS</span></span>

* <span data-ttu-id="e7e73-786">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-786">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e7e73-787">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-787">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e7e73-788">Advisor</span><span class="sxs-lookup"><span data-stu-id="e7e73-788">Advisor</span></span>

* <span data-ttu-id="e7e73-789">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-789">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e7e73-790">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-790">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e7e73-791">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-791">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e7e73-792">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-792">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e7e73-793">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-793">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-794">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-794">Appservice</span></span>

* <span data-ttu-id="e7e73-795">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-795">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e7e73-796">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-796">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e7e73-797">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="e7e73-797">Eventhubs</span></span>

* <span data-ttu-id="e7e73-798">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-798">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-799">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-799">Extension</span></span>

* <span data-ttu-id="e7e73-800">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-800">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-801">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-801">Interactive</span></span>

* <span data-ttu-id="e7e73-802">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="e7e73-802">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e7e73-803">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="e7e73-803">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e7e73-804">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-804">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e7e73-805">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-805">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-806">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-806">Monitor</span></span>

* <span data-ttu-id="e7e73-807">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-807">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e7e73-808">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-808">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e7e73-809">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-809">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e7e73-810">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-810">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-811">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-811">Network</span></span>

* <span data-ttu-id="e7e73-812">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-812">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e7e73-813">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="e7e73-813">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e7e73-814">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-814">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e7e73-815">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-815">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-816">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-816">Profile</span></span>

* <span data-ttu-id="e7e73-817">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-817">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e7e73-818">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-818">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-819">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-819">RDBMS</span></span>

* <span data-ttu-id="e7e73-820">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-820">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e7e73-821">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e7e73-821">Service Bus</span></span>

* <span data-ttu-id="e7e73-822">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-822">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-823">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-823">Storage</span></span>

* <span data-ttu-id="e7e73-824">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-824">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e7e73-825">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-825">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-826">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-826">VM</span></span>

* <span data-ttu-id="e7e73-827">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-827">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e7e73-828">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-828">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e7e73-829">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-829">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e7e73-830">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-830">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e7e73-831">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="e7e73-831">February 27, 2018</span></span>

<span data-ttu-id="e7e73-832">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e7e73-832">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-833">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-833">Core</span></span>

* <span data-ttu-id="e7e73-834">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-834">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e7e73-835">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-835">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e7e73-836">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-836">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-837">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-837">ACS</span></span>

* <span data-ttu-id="e7e73-838">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-838">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e7e73-839">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-839">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e7e73-840">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-840">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e7e73-841">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-841">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-842">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-842">Appservice</span></span>

* <span data-ttu-id="e7e73-843">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e7e73-843">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e7e73-844">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-844">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e7e73-845">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e7e73-845">Cognitive Services</span></span>

* <span data-ttu-id="e7e73-846">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-846">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e7e73-847">Consumption</span><span class="sxs-lookup"><span data-stu-id="e7e73-847">Consumption</span></span>

* <span data-ttu-id="e7e73-848">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-848">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e7e73-849">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-849">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-850">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-850">Container</span></span>

* <span data-ttu-id="e7e73-851">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-851">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-852">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-852">Network</span></span>

* <span data-ttu-id="e7e73-853">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-853">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-854">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-854">Resource</span></span>

* <span data-ttu-id="e7e73-855">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-855">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-856">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-856">Role</span></span>

* <span data-ttu-id="e7e73-857">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-857">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-858">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-858">SQL</span></span>

* <span data-ttu-id="e7e73-859">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-859">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-860">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-860">Storage</span></span>

* <span data-ttu-id="e7e73-861">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="e7e73-861">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-862">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-862">VM</span></span>

* <span data-ttu-id="e7e73-863">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-863">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e7e73-864">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="e7e73-864">February 13, 2018</span></span>

<span data-ttu-id="e7e73-865">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e7e73-865">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-866">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-866">Core</span></span>

* <span data-ttu-id="e7e73-867">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-867">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-868">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-868">ACS</span></span>

* <span data-ttu-id="e7e73-869">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-869">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e7e73-870">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-870">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e7e73-871">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-871">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e7e73-872">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="e7e73-872">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e7e73-873">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-873">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e7e73-874">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="e7e73-874">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e7e73-875">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-875">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e7e73-876">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-876">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-877">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-877">Appservice</span></span>

* <span data-ttu-id="e7e73-878">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-878">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e7e73-879">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-879">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e7e73-880">CDN</span><span class="sxs-lookup"><span data-stu-id="e7e73-880">CDN</span></span>

* <span data-ttu-id="e7e73-881">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-881">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-882">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-882">Container</span></span>

* <span data-ttu-id="e7e73-883">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-883">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e7e73-884">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-884">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e7e73-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e7e73-885">CosmosDB</span></span>

* <span data-ttu-id="e7e73-886">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-886">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-887">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-887">Extension</span></span>

* <span data-ttu-id="e7e73-888">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-888">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e7e73-889">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-889">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e7e73-890">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="e7e73-890">Feedback</span></span>

* <span data-ttu-id="e7e73-891">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-891">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-892">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-892">Interactive</span></span>

* <span data-ttu-id="e7e73-893">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-893">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e7e73-894">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-894">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-895">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-895">IoT</span></span>

* <span data-ttu-id="e7e73-896">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-896">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e7e73-897">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-897">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e7e73-898">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-898">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e7e73-899">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-899">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-900">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-900">Monitor</span></span>

* <span data-ttu-id="e7e73-901">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-901">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-902">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-902">Network</span></span>

* <span data-ttu-id="e7e73-903">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-903">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e7e73-904">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-904">Profile</span></span>

* <span data-ttu-id="e7e73-905">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-905">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-906">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-906">Resource</span></span>

* <span data-ttu-id="e7e73-907">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-907">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-908">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-908">Role</span></span>

* <span data-ttu-id="e7e73-909">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-909">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-910">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-910">SQL</span></span>

* <span data-ttu-id="e7e73-911">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-911">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e7e73-912">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-912">Added `sql db rename`</span></span>
* <span data-ttu-id="e7e73-913">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-913">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-914">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-914">Storage</span></span>

* <span data-ttu-id="e7e73-915">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-915">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-916">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-916">VM</span></span>

* <span data-ttu-id="e7e73-917">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-917">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e7e73-918">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-918">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e7e73-919">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="e7e73-919">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e7e73-920">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="e7e73-920">January 31, 2018</span></span>

<span data-ttu-id="e7e73-921">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e7e73-921">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-922">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-922">Core</span></span>

* <span data-ttu-id="e7e73-923">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-923">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e7e73-924">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-924">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e7e73-925">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-925">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e7e73-926">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="e7e73-926">Use `--verbose` to see</span></span>
* <span data-ttu-id="e7e73-927">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-927">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-928">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-928">ACS</span></span>

* <span data-ttu-id="e7e73-929">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-929">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e7e73-930">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="e7e73-930">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-931">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-931">Appservice</span></span>

* <span data-ttu-id="e7e73-932">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="e7e73-932">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e7e73-933">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-933">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e7e73-934">CDN</span><span class="sxs-lookup"><span data-stu-id="e7e73-934">CDN</span></span>

* <span data-ttu-id="e7e73-935">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-935">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e7e73-936">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e7e73-936">CosmosDB</span></span>

* <span data-ttu-id="e7e73-937">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-937">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-938">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-938">Interactive</span></span>

* <span data-ttu-id="e7e73-939">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-939">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-940">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-940">Network</span></span>

* <span data-ttu-id="e7e73-941">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-941">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e7e73-942">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-942">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e7e73-943">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-943">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e7e73-944">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-944">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e7e73-945">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-945">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e7e73-946">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="e7e73-946">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e7e73-947">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-947">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e7e73-948">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-948">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e7e73-949">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-949">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e7e73-950">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="e7e73-950">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-951">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-951">Profile</span></span>

* <span data-ttu-id="e7e73-952">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-952">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-953">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-953">Resource</span></span>

* <span data-ttu-id="e7e73-954">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-954">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-955">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-955">Storage</span></span>

* <span data-ttu-id="e7e73-956">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-956">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e7e73-957">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-957">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e7e73-958">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-958">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e7e73-959">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-959">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e7e73-960">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-960">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-961">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-961">VM</span></span>

* <span data-ttu-id="e7e73-962">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-962">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e7e73-963">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-963">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e7e73-964">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-964">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e7e73-965">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-965">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e7e73-966">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="e7e73-966">January 17, 2018</span></span>

<span data-ttu-id="e7e73-967">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e7e73-967">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-968">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-968">ACR</span></span>

* <span data-ttu-id="e7e73-969">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-969">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e7e73-970">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-970">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-971">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-971">ACS</span></span>

* <span data-ttu-id="e7e73-972">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-972">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e7e73-973">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-973">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-974">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-974">Appservice</span></span>

* <span data-ttu-id="e7e73-975">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-975">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e7e73-976">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-976">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e7e73-977">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-977">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e7e73-978">Backup</span><span class="sxs-lookup"><span data-stu-id="e7e73-978">Backup</span></span>

* <span data-ttu-id="e7e73-979">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-979">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e7e73-980">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-980">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e7e73-981">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-981">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e7e73-982">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-982">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e7e73-983">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-983">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-984">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-984">Batch</span></span>

* <span data-ttu-id="e7e73-985">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-985">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e7e73-986">클라우드</span><span class="sxs-lookup"><span data-stu-id="e7e73-986">Cloud</span></span>

* <span data-ttu-id="e7e73-987">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-987">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e7e73-988">Consumption</span><span class="sxs-lookup"><span data-stu-id="e7e73-988">Consumption</span></span>

* <span data-ttu-id="e7e73-989">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-989">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e7e73-990">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e7e73-990">Event Grid</span></span>

* <span data-ttu-id="e7e73-991">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-991">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e7e73-992">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-992">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e7e73-993">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-993">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e7e73-994">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="e7e73-994">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e7e73-995">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-995">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e7e73-996">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-996">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e7e73-997">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-997">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e7e73-998">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-998">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-999">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-999">Interactive</span></span>

* <span data-ttu-id="e7e73-1000">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1000">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e7e73-1001">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1001">Fixed errors on startup</span></span>
* <span data-ttu-id="e7e73-1002">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1002">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-1003">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-1003">IoT</span></span>

* <span data-ttu-id="e7e73-1004">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1004">Added support for device provisioning service</span></span>
* <span data-ttu-id="e7e73-1005">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1005">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e7e73-1006">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1006">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1007">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1007">Monitor</span></span>

* <span data-ttu-id="e7e73-1008">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1008">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e7e73-1009">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="e7e73-1009">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e7e73-1010">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1010">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1011">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1011">Network</span></span>

* <span data-ttu-id="e7e73-1012">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1012">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e7e73-1013">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1013">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-1014">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-1014">Profile</span></span>

* <span data-ttu-id="e7e73-1015">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1015">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-1016">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-1016">Role</span></span>

* <span data-ttu-id="e7e73-1017">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1017">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e7e73-1018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e7e73-1018">Service Fabric</span></span>

* <span data-ttu-id="e7e73-1019">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1019">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e7e73-1020">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1020">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1021">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1021">VM</span></span>

* <span data-ttu-id="e7e73-1022">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1022">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e7e73-1023">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1023">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e7e73-1024">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1024">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e7e73-1025">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1025">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e7e73-1026">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1026">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e7e73-1027">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1027">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e7e73-1028">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1028">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e7e73-1029">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1029">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e7e73-1030">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1030">December 19, 2017</span></span>

<span data-ttu-id="e7e73-1031">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e7e73-1031">Version 2.0.23</span></span>

* <span data-ttu-id="e7e73-1032">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1032">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-1033">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-1033">Container</span></span>

* <span data-ttu-id="e7e73-1034">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1034">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1035">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1035">Network</span></span>

* <span data-ttu-id="e7e73-1036">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1036">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e7e73-1037">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1037">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1038">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1038">Storage</span></span>

* <span data-ttu-id="e7e73-1039">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1039">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1040">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1040">VM</span></span>

* <span data-ttu-id="e7e73-1041">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1041">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e7e73-1042">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1042">December 5, 2017</span></span>

<span data-ttu-id="e7e73-1043">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e7e73-1043">Version 2.0.22</span></span>

* <span data-ttu-id="e7e73-1044">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1044">Removed `az component` commands.</span></span> <span data-ttu-id="e7e73-1045">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1045">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-1046">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1046">Core</span></span>
* <span data-ttu-id="e7e73-1047">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1047">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e7e73-1048">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1048">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1049">ACS</span></span>

* <span data-ttu-id="e7e73-1050">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1050">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e7e73-1051">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1051">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e7e73-1052">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1052">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e7e73-1053">Advisor</span><span class="sxs-lookup"><span data-stu-id="e7e73-1053">Advisor</span></span>

* <span data-ttu-id="e7e73-1054">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1054">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1055">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1055">Appservice</span></span>

* <span data-ttu-id="e7e73-1056">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1056">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e7e73-1057">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1057">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e7e73-1058">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1058">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e7e73-1059">Consumption</span><span class="sxs-lookup"><span data-stu-id="e7e73-1059">Consumption</span></span>

* <span data-ttu-id="e7e73-1060">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1060">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-1061">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-1061">Container</span></span>

* <span data-ttu-id="e7e73-1062">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1062">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1063">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1063">Monitor</span></span>

* <span data-ttu-id="e7e73-1064">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1064">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1065">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1065">Resource</span></span>

* <span data-ttu-id="e7e73-1066">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1066">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-1067">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-1067">Role</span></span>

* <span data-ttu-id="e7e73-1068">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1068">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e7e73-1069">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1069">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e7e73-1070">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1070">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1071">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1071">SQL</span></span>

* <span data-ttu-id="e7e73-1072">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1072">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e7e73-1073">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1073">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1074">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1074">VM</span></span>

* <span data-ttu-id="e7e73-1075">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1075">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e7e73-1076">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1076">November 14, 2017</span></span>

<span data-ttu-id="e7e73-1077">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e7e73-1077">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-1078">ACR</span></span>

* <span data-ttu-id="e7e73-1079">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1079">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e7e73-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1080">ACS</span></span>

* <span data-ttu-id="e7e73-1081">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1081">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e7e73-1082">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="e7e73-1082">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e7e73-1083">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1083">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e7e73-1084">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1084">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e7e73-1085">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1085">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1086">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1086">Appservice</span></span>

* <span data-ttu-id="e7e73-1087">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1087">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e7e73-1088">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1088">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e7e73-1089">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1089">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e7e73-1090">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1090">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e7e73-1091">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1091">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e7e73-1092">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1092">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-1093">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-1093">Batch</span></span>

* <span data-ttu-id="e7e73-1094">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1094">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e7e73-1095">Batchai</span><span class="sxs-lookup"><span data-stu-id="e7e73-1095">Batchai</span></span>

* <span data-ttu-id="e7e73-1096">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1096">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e7e73-1097">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1097">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e7e73-1098">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1098">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e7e73-1099">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1099">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e7e73-1100">클라우드</span><span class="sxs-lookup"><span data-stu-id="e7e73-1100">Cloud</span></span>

* <span data-ttu-id="e7e73-1101">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1101">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-1102">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-1102">Container</span></span>

* <span data-ttu-id="e7e73-1103">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1103">Added support to open multiple ports</span></span>
* <span data-ttu-id="e7e73-1104">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1104">Added container group restart policy</span></span>
* <span data-ttu-id="e7e73-1105">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1105">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e7e73-1106">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="e7e73-1106">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e7e73-1107">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e7e73-1107">Data Lake Analytics</span></span>

* <span data-ttu-id="e7e73-1108">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1108">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e7e73-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e7e73-1109">Data Lake Store</span></span>

* <span data-ttu-id="e7e73-1110">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1110">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-1111">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-1111">Extension</span></span>

* <span data-ttu-id="e7e73-1112">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1112">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e7e73-1113">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1113">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-1114">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-1114">IoT</span></span>

* <span data-ttu-id="e7e73-1115">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1115">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1116">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1116">Monitor</span></span>

* <span data-ttu-id="e7e73-1117">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1117">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1118">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1118">Network</span></span>

* <span data-ttu-id="e7e73-1119">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1119">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e7e73-1120">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1120">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e7e73-1121">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1121">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e7e73-1122">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1122">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e7e73-1123">예약</span><span class="sxs-lookup"><span data-stu-id="e7e73-1123">Reservations</span></span>

* <span data-ttu-id="e7e73-1124">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1124">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1125">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1125">Resource</span></span>

* <span data-ttu-id="e7e73-1126">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1126">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1127">SQL</span></span>

* <span data-ttu-id="e7e73-1128">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1128">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1129">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1129">Storage</span></span>

* <span data-ttu-id="e7e73-1130">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1130">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e7e73-1131">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1131">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e7e73-1132">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1132">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e7e73-1133">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="e7e73-1133">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e7e73-1134">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1134">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e7e73-1135">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1135">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e7e73-1136">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1136">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1137">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1137">VM</span></span>

* <span data-ttu-id="e7e73-1138">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1138">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e7e73-1139">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1139">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e7e73-1140">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1140">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e7e73-1141">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1141">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e7e73-1142">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1142">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e7e73-1143">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1143">October 24, 2017</span></span>

<span data-ttu-id="e7e73-1144">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e7e73-1144">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-1145">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1145">Core</span></span>

* <span data-ttu-id="e7e73-1146">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1146">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-1147">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-1147">ACR</span></span>

* <span data-ttu-id="e7e73-1148">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1148">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e7e73-1149">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1149">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e7e73-1150">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1150">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1151">ACS</span></span>

* <span data-ttu-id="e7e73-1152">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1152">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e7e73-1153">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1153">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1154">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1154">Appservice</span></span>

* <span data-ttu-id="e7e73-1155">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1155">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e7e73-1156">구성 요소</span><span class="sxs-lookup"><span data-stu-id="e7e73-1156">Component</span></span>

* <span data-ttu-id="e7e73-1157">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1157">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1158">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1158">Monitor</span></span>

* <span data-ttu-id="e7e73-1159">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1159">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1160">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1160">Resource</span></span>

* <span data-ttu-id="e7e73-1161">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1161">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e7e73-1162">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1162">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1163">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1163">VM</span></span>

* <span data-ttu-id="e7e73-1164">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1164">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e7e73-1165">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1165">October 9, 2017</span></span>

<span data-ttu-id="e7e73-1166">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e7e73-1166">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-1167">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1167">Core</span></span>

* <span data-ttu-id="e7e73-1168">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1168">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1169">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1169">Appservice</span></span>

* <span data-ttu-id="e7e73-1170">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1170">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-1171">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-1171">Batch</span></span>

* <span data-ttu-id="e7e73-1172">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1172">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e7e73-1173">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1173">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e7e73-1174">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1174">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e7e73-1175">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1175">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e7e73-1176">Batchai</span><span class="sxs-lookup"><span data-stu-id="e7e73-1176">Batchai</span></span>

* <span data-ttu-id="e7e73-1177">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1177">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-1178">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e7e73-1178">Keyvault</span></span>

* <span data-ttu-id="e7e73-1179">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1179">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e7e73-1180">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1180">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e7e73-1181">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1181">Network</span></span>

* <span data-ttu-id="e7e73-1182">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1182">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e7e73-1183">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1183">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1184">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1184">Resource</span></span>

* <span data-ttu-id="e7e73-1185">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1185">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e7e73-1186">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1186">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e7e73-1187">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1187">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e7e73-1188">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1188">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1189">Sql</span><span class="sxs-lookup"><span data-stu-id="e7e73-1189">Sql</span></span>

* <span data-ttu-id="e7e73-1190">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1190">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e7e73-1191">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1191">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e7e73-1192">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1192">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1193">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1193">Storage</span></span>

* <span data-ttu-id="e7e73-1194">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1194">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1195">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1195">Vm</span></span>

* <span data-ttu-id="e7e73-1196">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1196">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e7e73-1197">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1197">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e7e73-1198">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1198">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e7e73-1199">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1199">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e7e73-1200">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1200">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e7e73-1201">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1201">September 22, 2017</span></span>

<span data-ttu-id="e7e73-1202">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e7e73-1202">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1203">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1203">Resource</span></span>

* <span data-ttu-id="e7e73-1204">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1204">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e7e73-1205">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1205">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e7e73-1206">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1206">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e7e73-1207">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1207">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1208">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1208">Network</span></span>

* <span data-ttu-id="e7e73-1209">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1209">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e7e73-1210">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1210">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e7e73-1211">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1211">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e7e73-1212">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1212">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e7e73-1213">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1213">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e7e73-1214">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1214">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e7e73-1215">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1215">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1216">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1216">Storage</span></span>

* <span data-ttu-id="e7e73-1217">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1217">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e7e73-1218">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e7e73-1218">Eventgrid</span></span>

* <span data-ttu-id="e7e73-1219">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="e7e73-1219">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1220">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1220">SQL</span></span>

* <span data-ttu-id="e7e73-1221">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1221">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e7e73-1222">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1222">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e7e73-1223">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1223">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-1224">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e7e73-1224">Keyvault</span></span>

* <span data-ttu-id="e7e73-1225">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1225">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1226">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1226">VM</span></span>

* <span data-ttu-id="e7e73-1227">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1227">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e7e73-1228">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e7e73-1228">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e7e73-1229">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1229">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e7e73-1230">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1230">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e7e73-1231">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1231">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e7e73-1232">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1232">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1233">ACS</span></span>

* <span data-ttu-id="e7e73-1234">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1234">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1235">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1235">Appservice</span></span>

* <span data-ttu-id="e7e73-1236">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1236">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e7e73-1237">Backup</span><span class="sxs-lookup"><span data-stu-id="e7e73-1237">Backup</span></span>

* <span data-ttu-id="e7e73-1238">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1238">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e7e73-1239">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1239">September 11, 2017</span></span>

<span data-ttu-id="e7e73-1240">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e7e73-1240">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e7e73-1241">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1241">Core</span></span>

* <span data-ttu-id="e7e73-1242">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1242">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e7e73-1243">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1243">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1244">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1244">Acs</span></span>

* <span data-ttu-id="e7e73-1245">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1245">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e7e73-1246">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1246">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1247">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1247">Appservice</span></span>

* <span data-ttu-id="e7e73-1248">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1248">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e7e73-1249">CDN</span><span class="sxs-lookup"><span data-stu-id="e7e73-1249">CDN</span></span>

* <span data-ttu-id="e7e73-1250">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1250">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e7e73-1251">내선 번호</span><span class="sxs-lookup"><span data-stu-id="e7e73-1251">Extension</span></span>

* <span data-ttu-id="e7e73-1252">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1252">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-1253">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e7e73-1253">Keyvault</span></span>

* <span data-ttu-id="e7e73-1254">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1254">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1255">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1255">Network</span></span>

* <span data-ttu-id="e7e73-1256">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1256">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e7e73-1257">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1257">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e7e73-1258">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1258">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e7e73-1259">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1259">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e7e73-1260">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1260">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1261">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1261">Resource</span></span>

* <span data-ttu-id="e7e73-1262">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1262">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e7e73-1263">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1263">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e7e73-1264">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1264">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e7e73-1265">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="e7e73-1265">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1266">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1266">SQL</span></span>

* <span data-ttu-id="e7e73-1267">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1267">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1268">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1268">VM</span></span>

* <span data-ttu-id="e7e73-1269">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1269">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e7e73-1270">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1270">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e7e73-1271">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1271">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e7e73-1272">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1272">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e7e73-1273">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1273">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e7e73-1274">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1274">August 31, 2017</span></span>

<span data-ttu-id="e7e73-1275">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e7e73-1275">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-1276">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e7e73-1276">Keyvault</span></span>

* <span data-ttu-id="e7e73-1277">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1277">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e7e73-1278">Sf</span><span class="sxs-lookup"><span data-stu-id="e7e73-1278">Sf</span></span>

* <span data-ttu-id="e7e73-1279">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1279">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1280">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1280">Storage</span></span>

* <span data-ttu-id="e7e73-1281">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1281">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e7e73-1282">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1282">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e7e73-1283">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1283">August 28, 2017</span></span>

<span data-ttu-id="e7e73-1284">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e7e73-1284">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e7e73-1285">CLI</span><span class="sxs-lookup"><span data-stu-id="e7e73-1285">CLI</span></span>

* <span data-ttu-id="e7e73-1286">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1286">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1287">ACS</span></span>

* <span data-ttu-id="e7e73-1288">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1288">Corrected preview regions</span></span>
* <span data-ttu-id="e7e73-1289">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1289">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e7e73-1290">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1290">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1291">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1291">Appservice</span></span>

* <span data-ttu-id="e7e73-1292">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1292">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e7e73-1293">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1293">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e7e73-1294">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1294">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e7e73-1295">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1295">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e7e73-1296">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1296">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-1297">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-1297">IoT</span></span>

* <span data-ttu-id="e7e73-1298">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1298">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1299">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1299">Network</span></span>

* <span data-ttu-id="e7e73-1300">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1300">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e7e73-1301">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1301">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e7e73-1302">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1302">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e7e73-1303">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1303">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e7e73-1304">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1304">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-1305">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-1305">Profile</span></span>

* <span data-ttu-id="e7e73-1306">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1306">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e7e73-1307">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e7e73-1307">Service Fabric</span></span>

* <span data-ttu-id="e7e73-1308">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1308">Preview release</span></span>
* <span data-ttu-id="e7e73-1309">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1309">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e7e73-1310">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1310">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e7e73-1311">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1311">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1312">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1312">Storage</span></span>

* <span data-ttu-id="e7e73-1313">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1313">Enabled setting blob tier</span></span>
* <span data-ttu-id="e7e73-1314">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1314">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e7e73-1315">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1315">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e7e73-1316">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1316">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e7e73-1317">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1317">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e7e73-1318">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1318">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1319">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1319">VM</span></span>

* <span data-ttu-id="e7e73-1320">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1320">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e7e73-1321">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1321">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e7e73-1322">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1322">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e7e73-1323">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1323">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e7e73-1324">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1324">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e7e73-1325">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1325">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e7e73-1326">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1326">August 15, 2017</span></span>

<span data-ttu-id="e7e73-1327">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e7e73-1327">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1328">ACS</span></span>

* <span data-ttu-id="e7e73-1329">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1329">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1330">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1330">Appservice</span></span>

* <span data-ttu-id="e7e73-1331">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1331">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e7e73-1332">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e7e73-1332">Event Grid</span></span>

* <span data-ttu-id="e7e73-1333">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1333">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e7e73-1334">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1334">August 11, 2017</span></span>

<span data-ttu-id="e7e73-1335">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e7e73-1335">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1336">ACS</span></span>

* <span data-ttu-id="e7e73-1337">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1337">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-1338">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-1338">Batch</span></span>

* <span data-ttu-id="e7e73-1339">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1339">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e7e73-1340">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1340">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e7e73-1341">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1341">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e7e73-1342">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1342">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e7e73-1343">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1343">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e7e73-1344">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1344">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e7e73-1345">구성 요소</span><span class="sxs-lookup"><span data-stu-id="e7e73-1345">Component</span></span>

* <span data-ttu-id="e7e73-1346">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1346">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e7e73-1347">컨테이너</span><span class="sxs-lookup"><span data-stu-id="e7e73-1347">Container</span></span>

* <span data-ttu-id="e7e73-1348">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1348">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e7e73-1349">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e7e73-1349">Data Lake Store</span></span>

* <span data-ttu-id="e7e73-1350">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1350">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e7e73-1351">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e7e73-1351">Event Grid</span></span>

* <span data-ttu-id="e7e73-1352">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1352">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1353">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1353">Network</span></span>

* <span data-ttu-id="e7e73-1354">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1354">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e7e73-1355">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1355">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e7e73-1356">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1356">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e7e73-1357">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1357">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-1358">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-1358">Profile</span></span>

* <span data-ttu-id="e7e73-1359">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1359">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1360">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1360">Storage</span></span>

* <span data-ttu-id="e7e73-1361">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1361">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1362">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1362">VM</span></span>

* <span data-ttu-id="e7e73-1363">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1363">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e7e73-1364">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1364">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e7e73-1365">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1365">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e7e73-1366">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1366">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e7e73-1367">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1367">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e7e73-1368">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1368">July 28, 2017</span></span>

<span data-ttu-id="e7e73-1369">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e7e73-1369">Version 2.0.12</span></span>

* <span data-ttu-id="e7e73-1370">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1370">Added container commands</span></span>
* <span data-ttu-id="e7e73-1371">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1371">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e7e73-1372">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1372">Core</span></span>

* <span data-ttu-id="e7e73-1373">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1373">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e7e73-1374">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1374">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e7e73-1375">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1375">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e7e73-1376">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1376">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e7e73-1377">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="e7e73-1377">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e7e73-1378">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1378">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e7e73-1379">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1379">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e7e73-1380">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1380">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e7e73-1381">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1381">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e7e73-1382">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1382">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e7e73-1383">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="e7e73-1383">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e7e73-1384">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1384">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e7e73-1385">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1385">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e7e73-1386">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1386">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e7e73-1387">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1387">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e7e73-1388">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1388">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e7e73-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="e7e73-1389">ACR</span></span>

* <span data-ttu-id="e7e73-1390">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1390">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e7e73-1391">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1391">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e7e73-1392">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1392">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e7e73-1393">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1393">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e7e73-1394">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1394">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e7e73-1395">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1395">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1396">ACS</span></span>

* <span data-ttu-id="e7e73-1397">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1397">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1398">App Service</span><span class="sxs-lookup"><span data-stu-id="e7e73-1398">Appservice</span></span>

* <span data-ttu-id="e7e73-1399">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1399">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e7e73-1400">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1400">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e7e73-1401">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1401">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e7e73-1402">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1402">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e7e73-1403">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1403">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e7e73-1404">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1404">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e7e73-1405">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1405">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e7e73-1406">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1406">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e7e73-1407">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1407">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e7e73-1408">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1408">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e7e73-1409">Batch</span><span class="sxs-lookup"><span data-stu-id="e7e73-1409">Batch</span></span>

* <span data-ttu-id="e7e73-1410">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1410">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e7e73-1411">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1411">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e7e73-1412">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1412">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e7e73-1413">CDN</span><span class="sxs-lookup"><span data-stu-id="e7e73-1413">CDN</span></span>

* <span data-ttu-id="e7e73-1414">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1414">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e7e73-1415">클라우드</span><span class="sxs-lookup"><span data-stu-id="e7e73-1415">Cloud</span></span>

* <span data-ttu-id="e7e73-1416">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1416">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e7e73-1417">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1417">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e7e73-1418">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1418">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e7e73-1419">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1419">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e7e73-1420">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1420">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e7e73-1421">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e7e73-1421">CosmosDB</span></span>

* <span data-ttu-id="e7e73-1422">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1422">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e7e73-1423">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1423">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e7e73-1424">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e7e73-1424">Data Lake Analytics</span></span>

* <span data-ttu-id="e7e73-1425">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1425">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e7e73-1426">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1426">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e7e73-1427">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1427">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e7e73-1428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e7e73-1428">Data Lake Store</span></span>

* <span data-ttu-id="e7e73-1429">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1429">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e7e73-1430">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1430">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e7e73-1431">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1431">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e7e73-1432">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="e7e73-1432">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e7e73-1433">대화형</span><span class="sxs-lookup"><span data-stu-id="e7e73-1433">Interactive</span></span>

* <span data-ttu-id="e7e73-1434">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1434">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e7e73-1435">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1435">Increased test coverage</span></span>
* <span data-ttu-id="e7e73-1436">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1436">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e7e73-1437">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1437">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e7e73-1438">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1438">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e7e73-1439">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1439">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e7e73-1440">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1440">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e7e73-1441">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1441">Added `--progress` flag</span></span>
* <span data-ttu-id="e7e73-1442">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1442">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e7e73-1443">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1443">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e7e73-1444">IoT</span><span class="sxs-lookup"><span data-stu-id="e7e73-1444">IoT</span></span>

* <span data-ttu-id="e7e73-1445">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1445">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e7e73-1446">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1446">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e7e73-1447">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1447">Key vault</span></span>

* <span data-ttu-id="e7e73-1448">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="e7e73-1448">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e7e73-1449">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1449">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e7e73-1450">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1450">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e7e73-1451">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1451">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e7e73-1452">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1452">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e7e73-1453">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1453">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e7e73-1454">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1454">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e7e73-1455">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1455">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e7e73-1456">랩</span><span class="sxs-lookup"><span data-stu-id="e7e73-1456">Lab</span></span>

* <span data-ttu-id="e7e73-1457">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1457">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e7e73-1458">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1458">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1459">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1459">Monitor</span></span>

* <span data-ttu-id="e7e73-1460">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1460">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e7e73-1461">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1461">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e7e73-1462">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1462">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e7e73-1463">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1463">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e7e73-1464">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1464">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e7e73-1465">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="e7e73-1465">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e7e73-1466">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1466">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e7e73-1467">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1467">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e7e73-1468">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1468">`location` no longer required</span></span>
  * <span data-ttu-id="e7e73-1469">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1469">Add name and ID support for target</span></span>
  * <span data-ttu-id="e7e73-1470">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1470">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e7e73-1471">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1471">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e7e73-1472">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1472">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e7e73-1473">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1473">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e7e73-1474">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1474">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e7e73-1475">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1475">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1476">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1476">Network</span></span>

* <span data-ttu-id="e7e73-1477">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1477">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e7e73-1478">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1478">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e7e73-1479">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1479">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e7e73-1480">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1480">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e7e73-1481">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1481">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e7e73-1482">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1482">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e7e73-1483">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1483">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e7e73-1484">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1484">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e7e73-1485">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1485">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e7e73-1486">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1486">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e7e73-1487">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1487">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e7e73-1488">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1488">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e7e73-1489">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1489">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e7e73-1490">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e7e73-1490">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e7e73-1491">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1491">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e7e73-1492">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1492">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e7e73-1493">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1493">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e7e73-1494">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1494">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e7e73-1495">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1495">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e7e73-1496">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1496">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e7e73-1497">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1497">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e7e73-1498">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1498">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e7e73-1499">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1499">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e7e73-1500">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1500">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e7e73-1501">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1501">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e7e73-1502">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1502">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e7e73-1503">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1503">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-1504">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-1504">Profile</span></span>

* <span data-ttu-id="e7e73-1505">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1505">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e7e73-1506">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1506">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e7e73-1507">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1507">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e7e73-1508">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1508">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e7e73-1509">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1509">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e7e73-1510">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1510">RDBMS</span></span>

* <span data-ttu-id="e7e73-1511">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1511">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e7e73-1512">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1512">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e7e73-1513">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1513">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e7e73-1514">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1514">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1515">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1515">Resource</span></span>

* <span data-ttu-id="e7e73-1516">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1516">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e7e73-1517">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1517">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e7e73-1518">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1518">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e7e73-1519">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1519">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e7e73-1520">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1520">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e7e73-1521">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1521">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e7e73-1522">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1522">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e7e73-1523">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1523">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-1524">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-1524">Role</span></span>

* <span data-ttu-id="e7e73-1525">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1525">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e7e73-1526">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1526">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e7e73-1527">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1527">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e7e73-1528">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1528">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e7e73-1529">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1529">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e7e73-1530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e7e73-1530">Service Fabric</span></span>
* <span data-ttu-id="e7e73-1531">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="e7e73-1531">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e7e73-1532">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1532">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e7e73-1533">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1533">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1534">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1534">SQL</span></span>

* <span data-ttu-id="e7e73-1535">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1535">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e7e73-1536">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1536">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e7e73-1537">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1537">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1538">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1538">Storage</span></span>

* <span data-ttu-id="e7e73-1539">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1539">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e7e73-1540">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1540">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e7e73-1541">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1541">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e7e73-1542">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1542">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e7e73-1543">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1543">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e7e73-1544">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1544">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1545">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1545">VM</span></span>

* <span data-ttu-id="e7e73-1546">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1546">Support configuring nsg</span></span>
* <span data-ttu-id="e7e73-1547">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1547">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e7e73-1548">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1548">Support managed service identities</span></span>
* <span data-ttu-id="e7e73-1549">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1549">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e7e73-1550">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1550">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e7e73-1551">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1551">May 10, 2017</span></span>

<span data-ttu-id="e7e73-1552">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e7e73-1552">Version 2.0.6</span></span>

* <span data-ttu-id="e7e73-1553">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="e7e73-1553">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e7e73-1554">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1554">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e7e73-1555">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1555">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e7e73-1556">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1556">Include Cognitive Services module</span></span>
* <span data-ttu-id="e7e73-1557">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1557">Include Service Fabric module</span></span>
* <span data-ttu-id="e7e73-1558">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="e7e73-1558">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e7e73-1559">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1559">Add support for CDN commands</span></span>
* <span data-ttu-id="e7e73-1560">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-1560">Remove Container module</span></span>
* <span data-ttu-id="e7e73-1561">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1561">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e7e73-1562">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1562">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e7e73-1563">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1563">Core</span></span>

* <span data-ttu-id="e7e73-1564">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="e7e73-1564">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e7e73-1565">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1565">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e7e73-1566">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1566">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e7e73-1567">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1567">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e7e73-1568">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1568">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e7e73-1569">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1569">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e7e73-1570">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1570">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e7e73-1571">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1571">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e7e73-1572">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1572">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e7e73-1573">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="e7e73-1573">core: Improved performance</span></span>
* <span data-ttu-id="e7e73-1574">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1574">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e7e73-1575">core: 클라우드 구성 - '관리' 엔드포인트를 설정하지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1575">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1576">ACS</span></span>

* <span data-ttu-id="e7e73-1577">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1577">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e7e73-1578">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="e7e73-1578">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e7e73-1579">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="e7e73-1579">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e7e73-1580">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1580">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1581">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-1581">AppService</span></span>

* <span data-ttu-id="e7e73-1582">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1582">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e7e73-1583">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1583">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e7e73-1584">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1584">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e7e73-1585">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="e7e73-1585">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e7e73-1586">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="e7e73-1586">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e7e73-1587">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1587">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e7e73-1588">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1588">support slot swap with preview</span></span>
* <span data-ttu-id="e7e73-1589">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1589">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e7e73-1590">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1590">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e7e73-1591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e7e73-1591">CosmosDB</span></span>

* <span data-ttu-id="e7e73-1592">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="e7e73-1592">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e7e73-1593">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1593">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e7e73-1594">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1594">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e7e73-1595">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1595">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e7e73-1596">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e7e73-1596">Data Lake Analytics</span></span>

* <span data-ttu-id="e7e73-1597">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1597">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e7e73-1598">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1598">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e7e73-1599">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1599">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e7e73-1600">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="e7e73-1600">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e7e73-1601">테이블</span><span class="sxs-lookup"><span data-stu-id="e7e73-1601">Table</span></span>
  * <span data-ttu-id="e7e73-1602">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="e7e73-1602">Table valued function</span></span>
  * <span data-ttu-id="e7e73-1603">보기</span><span class="sxs-lookup"><span data-stu-id="e7e73-1603">View</span></span>
  * <span data-ttu-id="e7e73-1604">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1604">Table Statistics.</span></span> <span data-ttu-id="e7e73-1605">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1605">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e7e73-1606">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e7e73-1606">Data Lake Store</span></span>

* <span data-ttu-id="e7e73-1607">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="e7e73-1607">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e7e73-1608">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1608">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e7e73-1609">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1609">missed help for access show.</span></span> <span data-ttu-id="e7e73-1610">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1610">adding it.</span></span> <span data-ttu-id="e7e73-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e7e73-1612">찾기</span><span class="sxs-lookup"><span data-stu-id="e7e73-1612">Find</span></span>

* <span data-ttu-id="e7e73-1613">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="e7e73-1613">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e7e73-1614">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e7e73-1614">KeyVault</span></span>

* <span data-ttu-id="e7e73-1615">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1615">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e7e73-1616">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1616">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e7e73-1617">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1617">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e7e73-1618">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1618">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e7e73-1619">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1619">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e7e73-1620">랩</span><span class="sxs-lookup"><span data-stu-id="e7e73-1620">Lab</span></span>

* <span data-ttu-id="e7e73-1621">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1621">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e7e73-1622">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1622">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e7e73-1623">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="e7e73-1623">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e7e73-1624">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="e7e73-1624">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e7e73-1625">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1625">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e7e73-1626">모니터</span><span class="sxs-lookup"><span data-stu-id="e7e73-1626">Monitor</span></span>

* <span data-ttu-id="e7e73-1627">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1627">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e7e73-1628">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1628">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e7e73-1629">네트워크</span><span class="sxs-lookup"><span data-stu-id="e7e73-1629">Network</span></span>

* <span data-ttu-id="e7e73-1630">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1630">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e7e73-1631">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1631">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e7e73-1632">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1632">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e7e73-1633">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1633">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e7e73-1634">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1634">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e7e73-1635">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1635">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e7e73-1636">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1636">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e7e73-1637">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1637">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e7e73-1638">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1638">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e7e73-1639">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1639">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e7e73-1640">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="e7e73-1640">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e7e73-1641">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1641">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e7e73-1642">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1642">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e7e73-1643">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1643">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e7e73-1644">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1644">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e7e73-1645">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1645">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e7e73-1646">프로필</span><span class="sxs-lookup"><span data-stu-id="e7e73-1646">Profile</span></span>

* <span data-ttu-id="e7e73-1647">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1647">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e7e73-1648">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1648">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e7e73-1649">Redis</span><span class="sxs-lookup"><span data-stu-id="e7e73-1649">Redis</span></span>

* <span data-ttu-id="e7e73-1650">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1650">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e7e73-1651">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="e7e73-1651">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e7e73-1652">리소스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1652">Resource</span></span>

* <span data-ttu-id="e7e73-1653">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1653">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e7e73-1654">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1654">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e7e73-1655">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1655">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e7e73-1656">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1656">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e7e73-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e7e73-1658">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1658">Add docs for az lock update.</span></span> <span data-ttu-id="e7e73-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e7e73-1660">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1660">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e7e73-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e7e73-1662">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1662">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e7e73-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e7e73-1664">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1664">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e7e73-1665">역할</span><span class="sxs-lookup"><span data-stu-id="e7e73-1665">Role</span></span>

* <span data-ttu-id="e7e73-1666">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1666">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e7e73-1667">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1667">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e7e73-1668">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1668">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e7e73-1669">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="e7e73-1669">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e7e73-1670">SQL</span><span class="sxs-lookup"><span data-stu-id="e7e73-1670">SQL</span></span>

* <span data-ttu-id="e7e73-1671">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e7e73-1671">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e7e73-1672">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1672">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e7e73-1673">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1673">Storage</span></span>

* <span data-ttu-id="e7e73-1674">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="e7e73-1674">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e7e73-1675">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1675">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e7e73-1676">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1676">Add support for large block blob upload</span></span>
* <span data-ttu-id="e7e73-1677">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="e7e73-1677">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1678">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1678">VM</span></span>

* <span data-ttu-id="e7e73-1679">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="e7e73-1679">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e7e73-1680">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1680">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e7e73-1681">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e7e73-1681">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e7e73-1682">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e7e73-1682">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e7e73-1683">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1683">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e7e73-1684">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="e7e73-1684">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e7e73-1685">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1685">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e7e73-1686">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1686">April 3, 2017</span></span>

<span data-ttu-id="e7e73-1687">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e7e73-1687">Version 2.0.2</span></span>

<span data-ttu-id="e7e73-1688">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1688">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e7e73-1689">코어</span><span class="sxs-lookup"><span data-stu-id="e7e73-1689">Core</span></span>

* <span data-ttu-id="e7e73-1690">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="e7e73-1690">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e7e73-1691">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1691">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e7e73-1692">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1692">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e7e73-1693">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1693">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e7e73-1694">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1694">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e7e73-1695">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1695">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e7e73-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e7e73-1697">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1697">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e7e73-1698">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="e7e73-1698">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e7e73-1699">ACS</span><span class="sxs-lookup"><span data-stu-id="e7e73-1699">ACS</span></span>

* <span data-ttu-id="e7e73-1700">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1700">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e7e73-1701">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1701">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e7e73-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e7e73-1703">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1703">Add support for windows clusters.</span></span> <span data-ttu-id="e7e73-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e7e73-1705">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1705">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e7e73-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e7e73-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="e7e73-1707">AppService</span></span>

* <span data-ttu-id="e7e73-1708">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1708">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e7e73-1709">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1709">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e7e73-1710">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1710">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e7e73-1711">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1711">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e7e73-1712">DataLake</span><span class="sxs-lookup"><span data-stu-id="e7e73-1712">DataLake</span></span>

* <span data-ttu-id="e7e73-1713">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1713">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e7e73-1714">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="e7e73-1714">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e7e73-1715">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="e7e73-1715">DocuemntDB</span></span>

* <span data-ttu-id="e7e73-1716">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1716">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e7e73-1717">VM</span><span class="sxs-lookup"><span data-stu-id="e7e73-1717">VM</span></span>

* <span data-ttu-id="e7e73-1718">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1718">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e7e73-1719">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1719">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e7e73-1720">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1720">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e7e73-1721">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1721">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e7e73-1722">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1722">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e7e73-1723">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1723">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e7e73-1724">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e7e73-1724">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e7e73-1725">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="e7e73-1725">February 27, 2017</span></span>

<span data-ttu-id="e7e73-1726">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e7e73-1726">Version 2.0.0</span></span>

<span data-ttu-id="e7e73-1727">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1727">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e7e73-1728">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1728">Container Service (acs)</span></span>
- <span data-ttu-id="e7e73-1729">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="e7e73-1729">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e7e73-1730">네트워킹</span><span class="sxs-lookup"><span data-stu-id="e7e73-1730">Networking</span></span>
- <span data-ttu-id="e7e73-1731">Storage</span><span class="sxs-lookup"><span data-stu-id="e7e73-1731">Storage</span></span>

<span data-ttu-id="e7e73-1732">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1732">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e7e73-1733">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1733">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e7e73-1734">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1734">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e7e73-1735">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1735">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e7e73-1736">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1736">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e7e73-1737">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e7e73-1737">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e7e73-1738">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="e7e73-1738">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e7e73-1739">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="e7e73-1739">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e7e73-1740">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="e7e73-1740">Provide feedback from the command line with the `az feedback` command</span></span>


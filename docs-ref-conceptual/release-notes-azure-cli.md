---
title: "Azure CLI 2.0 릴리스 정보"
description: "Azure CLI 2.0 최신 업데이트 알아보기"
keywords: "Azure CLI 2.0, 릴리스 정보"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 39e4710a29ac57730919b82ab76b9c9a4b9ca786
ms.sourcegitcommit: 43d4f838d132ab9bcfa59dbda3b544c06373b6a9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/22/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="bf2d3-104">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="bf2d3-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-15-2017"></a><span data-ttu-id="bf2d3-105">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-105">August 15, 2017</span></span>

<span data-ttu-id="bf2d3-106">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="bf2d3-106">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="bf2d3-107">ACS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-107">ACS</span></span>

* <span data-ttu-id="bf2d3-108">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-108">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="bf2d3-109">App Service</span><span class="sxs-lookup"><span data-stu-id="bf2d3-109">Appservice</span></span>

* <span data-ttu-id="bf2d3-110">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-110">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="bf2d3-111">Event Grid</span><span class="sxs-lookup"><span data-stu-id="bf2d3-111">Event Grid</span></span>

* <span data-ttu-id="bf2d3-112">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-112">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="bf2d3-113">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-113">August 11, 2017</span></span>

<span data-ttu-id="bf2d3-114">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="bf2d3-114">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="bf2d3-115">ACS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-115">ACS</span></span>

* <span data-ttu-id="bf2d3-116">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-116">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="bf2d3-117">배치</span><span class="sxs-lookup"><span data-stu-id="bf2d3-117">Batch</span></span>

* <span data-ttu-id="bf2d3-118">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-118">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="bf2d3-119">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-119">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="bf2d3-120">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-120">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="bf2d3-121">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-121">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="bf2d3-122">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-122">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="bf2d3-123">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-123">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="bf2d3-124">구성 요소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-124">Component</span></span>

* <span data-ttu-id="bf2d3-125">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-125">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="bf2d3-126">컨테이너</span><span class="sxs-lookup"><span data-stu-id="bf2d3-126">Container</span></span>

* <span data-ttu-id="bf2d3-127">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-127">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="bf2d3-128">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-128">Data Lake Store</span></span>

* <span data-ttu-id="bf2d3-129">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-129">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="bf2d3-130">Event Grid</span><span class="sxs-lookup"><span data-stu-id="bf2d3-130">Event Grid</span></span>

* <span data-ttu-id="bf2d3-131">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="bf2d3-131">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="bf2d3-132">네트워크</span><span class="sxs-lookup"><span data-stu-id="bf2d3-132">Network</span></span>

* <span data-ttu-id="bf2d3-133">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-133">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="bf2d3-134">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-134">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="bf2d3-135">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-135">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="bf2d3-136">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-136">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="bf2d3-137">프로필</span><span class="sxs-lookup"><span data-stu-id="bf2d3-137">Profile</span></span>

* <span data-ttu-id="bf2d3-138">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-138">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="bf2d3-139">저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-139">Storage</span></span>

* <span data-ttu-id="bf2d3-140">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-140">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="bf2d3-141">VM</span><span class="sxs-lookup"><span data-stu-id="bf2d3-141">VM</span></span>

* <span data-ttu-id="bf2d3-142">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-142">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="bf2d3-143">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-143">Exposed `list-skus` command</span></span>
* <span data-ttu-id="bf2d3-144">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-144">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="bf2d3-145">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-145">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="bf2d3-146">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-146">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="bf2d3-147">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-147">July 28, 2017</span></span>

<span data-ttu-id="bf2d3-148">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="bf2d3-148">Version 2.0.12</span></span>

* <span data-ttu-id="bf2d3-149">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-149">Added container commands</span></span>
* <span data-ttu-id="bf2d3-150">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-150">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="bf2d3-151">코어</span><span class="sxs-lookup"><span data-stu-id="bf2d3-151">Core</span></span>

* <span data-ttu-id="bf2d3-152">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-152">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="bf2d3-153">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-153">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="bf2d3-154">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-154">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="bf2d3-155">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-155">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="bf2d3-156">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="bf2d3-156">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="bf2d3-157">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-157">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="bf2d3-158">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-158">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bf2d3-159">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-159">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="bf2d3-160">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-160">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="bf2d3-161">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-161">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="bf2d3-162">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="bf2d3-162">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="bf2d3-163">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-163">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="bf2d3-164">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-164">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="bf2d3-165">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-165">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="bf2d3-166">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-166">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="bf2d3-167">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-167">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="bf2d3-168">ACR</span><span class="sxs-lookup"><span data-stu-id="bf2d3-168">ACR</span></span>

* <span data-ttu-id="bf2d3-169">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-169">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="bf2d3-170">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-170">Support SKU update for managed registries</span></span>
* <span data-ttu-id="bf2d3-171">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-171">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="bf2d3-172">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-172">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="bf2d3-173">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-173">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="bf2d3-174">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-174">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="bf2d3-175">ACS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-175">ACS</span></span>

* <span data-ttu-id="bf2d3-176">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-176">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="bf2d3-177">App Service</span><span class="sxs-lookup"><span data-stu-id="bf2d3-177">Appservice</span></span>

* <span data-ttu-id="bf2d3-178">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-178">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="bf2d3-179">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-179">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="bf2d3-180">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-180">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="bf2d3-181">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-181">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="bf2d3-182">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-182">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="bf2d3-183">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-183">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="bf2d3-184">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-184">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="bf2d3-185">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-185">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="bf2d3-186">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-186">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="bf2d3-187">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-187">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="bf2d3-188">배치</span><span class="sxs-lookup"><span data-stu-id="bf2d3-188">Batch</span></span>

* <span data-ttu-id="bf2d3-189">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-189">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="bf2d3-190">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-190">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="bf2d3-191">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-191">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="bf2d3-192">CDN</span><span class="sxs-lookup"><span data-stu-id="bf2d3-192">CDN</span></span>

* <span data-ttu-id="bf2d3-193">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-193">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="bf2d3-194">클라우드</span><span class="sxs-lookup"><span data-stu-id="bf2d3-194">Cloud</span></span>

* <span data-ttu-id="bf2d3-195">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-195">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="bf2d3-196">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-196">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="bf2d3-197">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-197">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="bf2d3-198">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-198">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="bf2d3-199">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-199">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf2d3-200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf2d3-200">CosmosDB</span></span>

* <span data-ttu-id="bf2d3-201">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-201">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="bf2d3-202">컬렉션 기본 TTL에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-202">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bf2d3-203">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="bf2d3-203">Data Lake Analytics</span></span>

* <span data-ttu-id="bf2d3-204">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-204">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="bf2d3-205">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-205">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="bf2d3-206">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-206">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bf2d3-207">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-207">Data Lake Store</span></span>

* <span data-ttu-id="bf2d3-208">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-208">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="bf2d3-209">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-209">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="bf2d3-210">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-210">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="bf2d3-211">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="bf2d3-211">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="bf2d3-212">대화형</span><span class="sxs-lookup"><span data-stu-id="bf2d3-212">Interactive</span></span>

* <span data-ttu-id="bf2d3-213">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-213">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="bf2d3-214">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-214">Increased test coverage</span></span>
* <span data-ttu-id="bf2d3-215">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-215">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="bf2d3-216">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-216">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="bf2d3-217">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-217">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="bf2d3-218">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-218">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="bf2d3-219">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-219">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bf2d3-220">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-220">Added `--progress` flag</span></span>
* <span data-ttu-id="bf2d3-221">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-221">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="bf2d3-222">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-222">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="bf2d3-223">IoT</span><span class="sxs-lookup"><span data-stu-id="bf2d3-223">IoT</span></span>

* <span data-ttu-id="bf2d3-224">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-224">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="bf2d3-225">(#3934)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-225">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="bf2d3-226">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="bf2d3-226">Key vault</span></span>

* <span data-ttu-id="bf2d3-227">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="bf2d3-227">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="bf2d3-228">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-228">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="bf2d3-229">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-229">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bf2d3-230">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-230">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bf2d3-231">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-231">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="bf2d3-232">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-232">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="bf2d3-233">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-233">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="bf2d3-234">(#3307)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-234">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="bf2d3-235">랩</span><span class="sxs-lookup"><span data-stu-id="bf2d3-235">Lab</span></span>

* <span data-ttu-id="bf2d3-236">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-236">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="bf2d3-237">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-237">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="bf2d3-238">모니터</span><span class="sxs-lookup"><span data-stu-id="bf2d3-238">Monitor</span></span>

* <span data-ttu-id="bf2d3-239">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-239">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="bf2d3-240">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-240">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="bf2d3-241">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-241">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="bf2d3-242">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-242">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="bf2d3-243">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-243">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="bf2d3-244">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="bf2d3-244">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="bf2d3-245">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-245">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="bf2d3-246">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-246">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="bf2d3-247">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-247">`location` no longer required</span></span>
  * <span data-ttu-id="bf2d3-248">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-248">Add name and ID support for target</span></span>
  * <span data-ttu-id="bf2d3-249">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-249">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="bf2d3-250">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-250">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="bf2d3-251">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-251">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="bf2d3-252">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-252">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="bf2d3-253">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-253">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="bf2d3-254">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-254">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="bf2d3-255">네트워크</span><span class="sxs-lookup"><span data-stu-id="bf2d3-255">Network</span></span>

* <span data-ttu-id="bf2d3-256">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-256">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="bf2d3-257">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-257">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="bf2d3-258">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-258">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="bf2d3-259">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-259">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="bf2d3-260">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-260">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="bf2d3-261">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-261">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="bf2d3-262">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-262">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="bf2d3-263">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-263">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="bf2d3-264">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-264">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="bf2d3-265">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-265">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="bf2d3-266">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-266">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="bf2d3-267">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-267">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="bf2d3-268">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-268">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="bf2d3-269">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bf2d3-269">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="bf2d3-270">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-270">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="bf2d3-271">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-271">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="bf2d3-272">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-272">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="bf2d3-273">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-273">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="bf2d3-274">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-274">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="bf2d3-275">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-275">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="bf2d3-276">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-276">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="bf2d3-277">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-277">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="bf2d3-278">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-278">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="bf2d3-279">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-279">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="bf2d3-280">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-280">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="bf2d3-281">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-281">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="bf2d3-282">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-282">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="bf2d3-283">프로필</span><span class="sxs-lookup"><span data-stu-id="bf2d3-283">Profile</span></span>

* <span data-ttu-id="bf2d3-284">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-284">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="bf2d3-285">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-285">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="bf2d3-286">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-286">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="bf2d3-287">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-287">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="bf2d3-288">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-288">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="bf2d3-289">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-289">RDBMS</span></span>

* <span data-ttu-id="bf2d3-290">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-290">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="bf2d3-291">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-291">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="bf2d3-292">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-292">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="bf2d3-293">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-293">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="bf2d3-294">리소스</span><span class="sxs-lookup"><span data-stu-id="bf2d3-294">Resource</span></span>

* <span data-ttu-id="bf2d3-295">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-295">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="bf2d3-296">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-296">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="bf2d3-297">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-297">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="bf2d3-298">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-298">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="bf2d3-299">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-299">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="bf2d3-300">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-300">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="bf2d3-301">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-301">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="bf2d3-302">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-302">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="bf2d3-303">역할</span><span class="sxs-lookup"><span data-stu-id="bf2d3-303">Role</span></span>

* <span data-ttu-id="bf2d3-304">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-304">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="bf2d3-305">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-305">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="bf2d3-306">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-306">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="bf2d3-307">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-307">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="bf2d3-308">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-308">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bf2d3-309">서비스 패브릭</span><span class="sxs-lookup"><span data-stu-id="bf2d3-309">Service Fabric</span></span>
* <span data-ttu-id="bf2d3-310">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="bf2d3-310">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="bf2d3-311">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-311">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="bf2d3-312">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-312">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="bf2d3-313">SQL</span><span class="sxs-lookup"><span data-stu-id="bf2d3-313">SQL</span></span>

* <span data-ttu-id="bf2d3-314">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-314">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="bf2d3-315">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-315">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="bf2d3-316">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-316">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="bf2d3-317">저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-317">Storage</span></span>

* <span data-ttu-id="bf2d3-318">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-318">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="bf2d3-319">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="bf2d3-319">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="bf2d3-320">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-320">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="bf2d3-321">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-321">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="bf2d3-322">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-322">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="bf2d3-323">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-323">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="bf2d3-324">VM</span><span class="sxs-lookup"><span data-stu-id="bf2d3-324">VM</span></span>

* <span data-ttu-id="bf2d3-325">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-325">Support configuring nsg</span></span>
* <span data-ttu-id="bf2d3-326">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-326">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="bf2d3-327">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-327">Support managed service identities</span></span>
* <span data-ttu-id="bf2d3-328">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-328">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="bf2d3-329">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-329">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="bf2d3-330">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-330">May 10, 2017</span></span>

<span data-ttu-id="bf2d3-331">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="bf2d3-331">Version 2.0.6</span></span>

* <span data-ttu-id="bf2d3-332">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="bf2d3-332">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="bf2d3-333">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-333">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="bf2d3-334">Data Lake Analytics 및 Data Lake Store 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-334">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="bf2d3-335">Cognitive Services 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-335">Include Cognitive Services module.</span></span>
* <span data-ttu-id="bf2d3-336">Service Fabric 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-336">Include Service Fabric module.</span></span>
* <span data-ttu-id="bf2d3-337">대화형 모듈(az-shell 이름 바꾸기)을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-337">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="bf2d3-338">CDN 명령에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-338">Add support for CDN commands.</span></span>
* <span data-ttu-id="bf2d3-339">컨테이너 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-339">Remove Container module.</span></span>
* <span data-ttu-id="bf2d3-340">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-340">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="bf2d3-341">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-341">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="bf2d3-342">코어</span><span class="sxs-lookup"><span data-stu-id="bf2d3-342">Core</span></span>

* <span data-ttu-id="bf2d3-343">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="bf2d3-343">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="bf2d3-344">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-344">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="bf2d3-345">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-345">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="bf2d3-346">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-346">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="bf2d3-347">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-347">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="bf2d3-348">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-348">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="bf2d3-349">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-349">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="bf2d3-350">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-350">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="bf2d3-351">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-351">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="bf2d3-352">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="bf2d3-352">core: Improved performance</span></span>
* <span data-ttu-id="bf2d3-353">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-353">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="bf2d3-354">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="bf2d3-354">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="bf2d3-355">ACS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-355">ACS</span></span>

* <span data-ttu-id="bf2d3-356">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="bf2d3-356">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="bf2d3-357">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="bf2d3-357">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="bf2d3-358">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="bf2d3-358">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="bf2d3-359">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-359">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="bf2d3-360">AppService</span><span class="sxs-lookup"><span data-stu-id="bf2d3-360">AppService</span></span>

* <span data-ttu-id="bf2d3-361">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-361">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="bf2d3-362">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-362">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="bf2d3-363">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-363">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="bf2d3-364">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="bf2d3-364">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="bf2d3-365">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="bf2d3-365">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="bf2d3-366">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-366">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="bf2d3-367">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-367">support slot swap with preview</span></span>
* <span data-ttu-id="bf2d3-368">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-368">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="bf2d3-369">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-369">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf2d3-370">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf2d3-370">CosmosDB</span></span>

* <span data-ttu-id="bf2d3-371">documentdb 모듈 이름을 cosmosdb로 바꿈</span><span class="sxs-lookup"><span data-stu-id="bf2d3-371">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="bf2d3-372">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-372">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="bf2d3-373">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-373">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="bf2d3-374">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="bf2d3-374">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bf2d3-375">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="bf2d3-375">Data Lake Analytics</span></span>

* <span data-ttu-id="bf2d3-376">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-376">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="bf2d3-377">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-377">Add support for new catalog item type: package.</span></span> <span data-ttu-id="bf2d3-378">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="bf2d3-378">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="bf2d3-379">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="bf2d3-379">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="bf2d3-380">테이블</span><span class="sxs-lookup"><span data-stu-id="bf2d3-380">Table</span></span>
  * <span data-ttu-id="bf2d3-381">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="bf2d3-381">Table valued function</span></span>
  * <span data-ttu-id="bf2d3-382">보기</span><span class="sxs-lookup"><span data-stu-id="bf2d3-382">View</span></span>
  * <span data-ttu-id="bf2d3-383">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-383">Table Statistics.</span></span> <span data-ttu-id="bf2d3-384">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-384">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bf2d3-385">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-385">Data Lake Store</span></span>

* <span data-ttu-id="bf2d3-386">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 대해 보다 나은 지원을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-386">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="bf2d3-387">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-387">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="bf2d3-388">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-388">missed help for access show.</span></span> <span data-ttu-id="bf2d3-389">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-389">adding it.</span></span> <span data-ttu-id="bf2d3-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="bf2d3-391">찾기</span><span class="sxs-lookup"><span data-stu-id="bf2d3-391">Find</span></span>

* <span data-ttu-id="bf2d3-392">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="bf2d3-392">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf2d3-393">KeyVault</span><span class="sxs-lookup"><span data-stu-id="bf2d3-393">KeyVault</span></span>

* <span data-ttu-id="bf2d3-394">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-394">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="bf2d3-395">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-395">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="bf2d3-396">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-396">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="bf2d3-397">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-397">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="bf2d3-398">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-398">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="bf2d3-399">랩</span><span class="sxs-lookup"><span data-stu-id="bf2d3-399">Lab</span></span>

* <span data-ttu-id="bf2d3-400">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-400">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="bf2d3-401">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-401">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="bf2d3-402">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-402">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="bf2d3-403">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-403">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="bf2d3-404">랩 내에서 비밀을 관리하는 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-404">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="bf2d3-405">모니터</span><span class="sxs-lookup"><span data-stu-id="bf2d3-405">Monitor</span></span>

* <span data-ttu-id="bf2d3-406">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-406">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="bf2d3-407">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-407">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="bf2d3-408">네트워크</span><span class="sxs-lookup"><span data-stu-id="bf2d3-408">Network</span></span>

* <span data-ttu-id="bf2d3-409">`network watcher test-connectivity` 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-409">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="bf2d3-410">`network watcher packet-capture create`에 대한 `--filters` 매개 변수 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-410">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="bf2d3-411">Application Gateway 연결 드레이닝에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-411">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="bf2d3-412">Application Gateway WAF 규칙 집합 구성에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-412">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="bf2d3-413">ExpressRoute 경로 필터 및 규칙에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-413">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="bf2d3-414">TrafficManager 지리적 라우팅에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-414">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="bf2d3-415">VPN 연결 정책 기반 트래픽 선택기에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-415">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="bf2d3-416">VPN 연결 IPSec 정책에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-416">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="bf2d3-417">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create`를 사용하여 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-417">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="bf2d3-418">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-418">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="bf2d3-419">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="bf2d3-419">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="bf2d3-420">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="bf2d3-420">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="bf2d3-421">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-421">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="bf2d3-422">레코드가 제대로 가져와지지 않는 `dns zone import`의 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-422">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="bf2d3-423">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-423">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="bf2d3-424">'network watcher' 미리 보기 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-424">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="bf2d3-425">프로필</span><span class="sxs-lookup"><span data-stu-id="bf2d3-425">Profile</span></span>

* <span data-ttu-id="bf2d3-426">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-426">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="bf2d3-427">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-427">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="bf2d3-428">Redis</span><span class="sxs-lookup"><span data-stu-id="bf2d3-428">Redis</span></span>

* <span data-ttu-id="bf2d3-429">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-429">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="bf2d3-430">'update-settings' 명령은 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-430">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="bf2d3-431">리소스</span><span class="sxs-lookup"><span data-stu-id="bf2d3-431">Resource</span></span>

* <span data-ttu-id="bf2d3-432">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-432">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="bf2d3-433">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-433">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="bf2d3-434">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-434">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="bf2d3-435">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-435">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="bf2d3-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="bf2d3-437">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-437">Add docs for az lock update.</span></span> <span data-ttu-id="bf2d3-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="bf2d3-439">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-439">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="bf2d3-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="bf2d3-441">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-441">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="bf2d3-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="bf2d3-443">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-443">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="bf2d3-444">역할</span><span class="sxs-lookup"><span data-stu-id="bf2d3-444">Role</span></span>

* <span data-ttu-id="bf2d3-445">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-445">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="bf2d3-446">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-446">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="bf2d3-447">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-447">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="bf2d3-448">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="bf2d3-448">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="bf2d3-449">SQL</span><span class="sxs-lookup"><span data-stu-id="bf2d3-449">SQL</span></span>

* <span data-ttu-id="bf2d3-450">az sql server list-usages 및 az sql db list-usages 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-450">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="bf2d3-451">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-451">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="bf2d3-452">저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-452">Storage</span></span>

* <span data-ttu-id="bf2d3-453">기본 위치를 `storage account create`에 대한 리소스 그룹 위치로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-453">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="bf2d3-454">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-454">Add support for incremental blob copy</span></span>
* <span data-ttu-id="bf2d3-455">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="bf2d3-455">Add support for large block blob upload</span></span>
* <span data-ttu-id="bf2d3-456">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="bf2d3-456">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="bf2d3-457">VM</span><span class="sxs-lookup"><span data-stu-id="bf2d3-457">VM</span></span>

* <span data-ttu-id="bf2d3-458">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="bf2d3-458">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="bf2d3-459">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-459">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="bf2d3-460">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="bf2d3-460">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="bf2d3-461">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="bf2d3-461">az vm/vmss disk</span></span>
  3. <span data-ttu-id="bf2d3-462">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-462">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="bf2d3-463">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="bf2d3-463">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="bf2d3-464">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-464">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="bf2d3-465">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-465">April 3, 2017</span></span>

<span data-ttu-id="bf2d3-466">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="bf2d3-466">Version 2.0.2</span></span>

<span data-ttu-id="bf2d3-467">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 출시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-467">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="bf2d3-468">코어</span><span class="sxs-lookup"><span data-stu-id="bf2d3-468">Core</span></span>

* <span data-ttu-id="bf2d3-469">기본 목록에 acr, 랩, 모니터 및 찾기 모듈을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-469">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="bf2d3-470">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-470">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="bf2d3-471">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-471">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="bf2d3-472">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-472">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bf2d3-473">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-473">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="bf2d3-474">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-474">Add prompting for missing template parameters.</span></span> <span data-ttu-id="bf2d3-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="bf2d3-476">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-476">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="bf2d3-477">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="bf2d3-477">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="bf2d3-478">ACS</span><span class="sxs-lookup"><span data-stu-id="bf2d3-478">ACS</span></span>

* <span data-ttu-id="bf2d3-479">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-479">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="bf2d3-480">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-480">Add support for ssh key password prompting.</span></span> <span data-ttu-id="bf2d3-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="bf2d3-482">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-482">Add support for windows clusters.</span></span> <span data-ttu-id="bf2d3-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="bf2d3-484">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-484">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="bf2d3-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="bf2d3-486">AppService</span><span class="sxs-lookup"><span data-stu-id="bf2d3-486">AppService</span></span>

* <span data-ttu-id="bf2d3-487">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-487">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="bf2d3-488">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-488">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="bf2d3-489">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-489">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="bf2d3-490">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-490">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="bf2d3-491">DataLake</span><span class="sxs-lookup"><span data-stu-id="bf2d3-491">DataLake</span></span>

* <span data-ttu-id="bf2d3-492">Data Lake Analytics 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-492">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="bf2d3-493">Data Lake Store 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-493">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="bf2d3-494">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="bf2d3-494">DocuemntDB</span></span>

* <span data-ttu-id="bf2d3-495">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-495">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="bf2d3-496">VM</span><span class="sxs-lookup"><span data-stu-id="bf2d3-496">VM</span></span>

* <span data-ttu-id="bf2d3-497">[Compute] 가상 컴퓨터 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-497">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="bf2d3-498">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-498">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="bf2d3-499">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-499">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="bf2d3-500">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-500">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bf2d3-501">가상 컴퓨터 확장 집합: vm의 인스턴스 보기를 나열하는 * 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-501">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="bf2d3-502">VM 및 가상 컴퓨터 확장 집합에 --secrets 추가([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-502">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="bf2d3-503">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="bf2d3-503">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="bf2d3-504">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="bf2d3-504">February 27, 2017</span></span>

<span data-ttu-id="bf2d3-505">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="bf2d3-505">Version 2.0.0</span></span>

<span data-ttu-id="bf2d3-506">Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-506">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="bf2d3-507">일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-507">General availability applies to these command modules:</span></span>
- <span data-ttu-id="bf2d3-508">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-508">Container Service (acs)</span></span>
- <span data-ttu-id="bf2d3-509">Compute(Resource Manager, VM, 가상 컴퓨터 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="bf2d3-509">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="bf2d3-510">네트워킹</span><span class="sxs-lookup"><span data-stu-id="bf2d3-510">Networking</span></span>
- <span data-ttu-id="bf2d3-511">저장소</span><span class="sxs-lookup"><span data-stu-id="bf2d3-511">Storage</span></span>

<span data-ttu-id="bf2d3-512">이러한 명령은 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-512">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="bf2d3-513">Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 개설할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-513">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="bf2d3-514">[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-514">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="bf2d3-515">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-515">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="bf2d3-516">CLI 버전을 확인하려면 `az --version`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-516">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="bf2d3-517">출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-517">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="bf2d3-518">일부 명령 모듈에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-518">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="bf2d3-519">이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-519">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="bf2d3-520">CLI 야간 미리 보기 빌드도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-520">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="bf2d3-521">자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-521">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="bf2d3-522">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-522">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="bf2d3-523">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="bf2d3-523">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="bf2d3-524">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-524">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="bf2d3-525">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공.</span><span class="sxs-lookup"><span data-stu-id="bf2d3-525">Provide feedback from the command line with the `az feedback` command.</span></span>


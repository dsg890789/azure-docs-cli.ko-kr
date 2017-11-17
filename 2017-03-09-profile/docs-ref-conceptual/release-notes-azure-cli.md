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
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="32e11-104">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="32e11-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="32e11-105">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="32e11-105">August 28, 2017</span></span>

<span data-ttu-id="32e11-106">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="32e11-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="32e11-107">CLI</span><span class="sxs-lookup"><span data-stu-id="32e11-107">CLI</span></span>

* <span data-ttu-id="32e11-108">`--version`에 법적 정보가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="32e11-109">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-109">ACS</span></span>

* <span data-ttu-id="32e11-110">미리 보기 지역이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-110">Corrected preview regions.</span></span>
* <span data-ttu-id="32e11-111">`dns_name_prefix`의 기본 형식이 올바르게 지정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="32e11-112">acs 명령 출력이 최적화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="32e11-113">App Service</span><span class="sxs-lookup"><span data-stu-id="32e11-113">Appservice</span></span>

* <span data-ttu-id="32e11-114">[주요 변경 내용] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="32e11-115">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="32e11-116">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="32e11-117">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="32e11-118">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="32e11-119">IoT</span><span class="sxs-lookup"><span data-stu-id="32e11-119">IoT</span></span>

* <span data-ttu-id="32e11-120">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="32e11-121">네트워크</span><span class="sxs-lookup"><span data-stu-id="32e11-121">Network</span></span>

* <span data-ttu-id="32e11-122">[주요 변경 내용] 이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="32e11-123">[주요 변경 내용] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="32e11-124">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="32e11-125">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="32e11-126">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="32e11-127">프로필</span><span class="sxs-lookup"><span data-stu-id="32e11-127">Profile</span></span>

* <span data-ttu-id="32e11-128">가상 컴퓨터의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="32e11-129">서비스 패브릭</span><span class="sxs-lookup"><span data-stu-id="32e11-129">Service Fabric</span></span>

* <span data-ttu-id="32e11-130">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="32e11-130">Preview release</span></span>
* <span data-ttu-id="32e11-131">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="32e11-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="32e11-132">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="32e11-133">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="32e11-134">저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-134">Storage</span></span>

* <span data-ttu-id="32e11-135">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="32e11-136">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="32e11-137">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="32e11-138">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="32e11-139">[주요 변경 내용] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="32e11-140">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="32e11-141">VM</span><span class="sxs-lookup"><span data-stu-id="32e11-141">VM</span></span>

* <span data-ttu-id="32e11-142">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="32e11-143">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="32e11-144">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="32e11-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="32e11-145">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="32e11-146">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="32e11-147">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="32e11-148">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="32e11-148">August 15, 2017</span></span>

<span data-ttu-id="32e11-149">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="32e11-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="32e11-150">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-150">ACS</span></span>

* <span data-ttu-id="32e11-151">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="32e11-152">App Service</span><span class="sxs-lookup"><span data-stu-id="32e11-152">Appservice</span></span>

* <span data-ttu-id="32e11-153">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="32e11-154">Event Grid</span><span class="sxs-lookup"><span data-stu-id="32e11-154">Event Grid</span></span>

* <span data-ttu-id="32e11-155">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="32e11-156">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="32e11-156">August 11, 2017</span></span>

<span data-ttu-id="32e11-157">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="32e11-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="32e11-158">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-158">ACS</span></span>

* <span data-ttu-id="32e11-159">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="32e11-160">배치</span><span class="sxs-lookup"><span data-stu-id="32e11-160">Batch</span></span>

* <span data-ttu-id="32e11-161">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="32e11-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="32e11-162">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="32e11-163">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="32e11-164">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="32e11-165">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="32e11-166">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="32e11-167">구성 요소</span><span class="sxs-lookup"><span data-stu-id="32e11-167">Component</span></span>

* <span data-ttu-id="32e11-168">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="32e11-169">컨테이너</span><span class="sxs-lookup"><span data-stu-id="32e11-169">Container</span></span>

* <span data-ttu-id="32e11-170">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="32e11-171">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-171">Data Lake Store</span></span>

* <span data-ttu-id="32e11-172">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="32e11-173">Event Grid</span><span class="sxs-lookup"><span data-stu-id="32e11-173">Event Grid</span></span>

* <span data-ttu-id="32e11-174">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="32e11-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="32e11-175">네트워크</span><span class="sxs-lookup"><span data-stu-id="32e11-175">Network</span></span>

* <span data-ttu-id="32e11-176">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="32e11-177">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="32e11-178">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="32e11-179">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="32e11-180">프로필</span><span class="sxs-lookup"><span data-stu-id="32e11-180">Profile</span></span>

* <span data-ttu-id="32e11-181">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="32e11-182">저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-182">Storage</span></span>

* <span data-ttu-id="32e11-183">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="32e11-184">VM</span><span class="sxs-lookup"><span data-stu-id="32e11-184">VM</span></span>

* <span data-ttu-id="32e11-185">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="32e11-186">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="32e11-187">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="32e11-188">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="32e11-189">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="32e11-190">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="32e11-190">July 28, 2017</span></span>

<span data-ttu-id="32e11-191">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="32e11-191">Version 2.0.12</span></span>

* <span data-ttu-id="32e11-192">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-192">Added container commands</span></span>
* <span data-ttu-id="32e11-193">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-193">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="32e11-194">코어</span><span class="sxs-lookup"><span data-stu-id="32e11-194">Core</span></span>

* <span data-ttu-id="32e11-195">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="32e11-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="32e11-196">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="32e11-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="32e11-197">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="32e11-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="32e11-198">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="32e11-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="32e11-199">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="32e11-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="32e11-200">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="32e11-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="32e11-201">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="32e11-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="32e11-202">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="32e11-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="32e11-203">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="32e11-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="32e11-204">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="32e11-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="32e11-205">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="32e11-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="32e11-206">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="32e11-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="32e11-207">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="32e11-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="32e11-208">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="32e11-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="32e11-209">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="32e11-210">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="32e11-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="32e11-211">ACR</span><span class="sxs-lookup"><span data-stu-id="32e11-211">ACR</span></span>

* <span data-ttu-id="32e11-212">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="32e11-213">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="32e11-214">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="32e11-215">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="32e11-216">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="32e11-217">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="32e11-218">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-218">ACS</span></span>

* <span data-ttu-id="32e11-219">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="32e11-220">App Service</span><span class="sxs-lookup"><span data-stu-id="32e11-220">Appservice</span></span>

* <span data-ttu-id="32e11-221">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="32e11-222">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="32e11-223">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="32e11-224">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="32e11-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="32e11-225">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="32e11-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="32e11-226">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="32e11-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="32e11-227">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="32e11-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="32e11-228">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="32e11-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="32e11-229">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="32e11-230">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="32e11-231">배치</span><span class="sxs-lookup"><span data-stu-id="32e11-231">Batch</span></span>

* <span data-ttu-id="32e11-232">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="32e11-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="32e11-233">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="32e11-234">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="32e11-235">CDN</span><span class="sxs-lookup"><span data-stu-id="32e11-235">CDN</span></span>

* <span data-ttu-id="32e11-236">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="32e11-237">클라우드</span><span class="sxs-lookup"><span data-stu-id="32e11-237">Cloud</span></span>

* <span data-ttu-id="32e11-238">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="32e11-239">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="32e11-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="32e11-240">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="32e11-241">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="32e11-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="32e11-242">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="32e11-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32e11-243">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32e11-243">CosmosDB</span></span>

* <span data-ttu-id="32e11-244">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="32e11-245">컬렉션 기본 TTL에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="32e11-246">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="32e11-246">Data Lake Analytics</span></span>

* <span data-ttu-id="32e11-247">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="32e11-248">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="32e11-249">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="32e11-250">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-250">Data Lake Store</span></span>

* <span data-ttu-id="32e11-251">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="32e11-252">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="32e11-253">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="32e11-254">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="32e11-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="32e11-255">대화형</span><span class="sxs-lookup"><span data-stu-id="32e11-255">Interactive</span></span>

* <span data-ttu-id="32e11-256">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="32e11-257">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-257">Increased test coverage</span></span>
* <span data-ttu-id="32e11-258">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="32e11-259">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="32e11-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="32e11-260">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="32e11-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="32e11-261">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="32e11-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="32e11-262">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="32e11-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="32e11-263">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-263">Added `--progress` flag</span></span>
* <span data-ttu-id="32e11-264">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="32e11-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="32e11-265">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="32e11-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="32e11-266">IoT</span><span class="sxs-lookup"><span data-stu-id="32e11-266">IoT</span></span>

* <span data-ttu-id="32e11-267">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="32e11-268">(#3934)</span><span class="sxs-lookup"><span data-stu-id="32e11-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="32e11-269">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="32e11-269">Key vault</span></span>

* <span data-ttu-id="32e11-270">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="32e11-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="32e11-271">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32e11-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="32e11-272">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32e11-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="32e11-273">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32e11-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="32e11-274">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="32e11-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="32e11-275">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="32e11-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="32e11-276">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="32e11-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="32e11-277">(#3307)</span><span class="sxs-lookup"><span data-stu-id="32e11-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="32e11-278">랩</span><span class="sxs-lookup"><span data-stu-id="32e11-278">Lab</span></span>

* <span data-ttu-id="32e11-279">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="32e11-280">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="32e11-281">모니터</span><span class="sxs-lookup"><span data-stu-id="32e11-281">Monitor</span></span>

* <span data-ttu-id="32e11-282">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="32e11-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="32e11-283">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="32e11-284">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="32e11-285">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="32e11-286">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="32e11-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="32e11-287">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="32e11-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="32e11-288">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="32e11-289">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="32e11-290">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-290">`location` no longer required</span></span>
  * <span data-ttu-id="32e11-291">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="32e11-292">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="32e11-293">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="32e11-294">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="32e11-295">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="32e11-296">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="32e11-297">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="32e11-298">네트워크</span><span class="sxs-lookup"><span data-stu-id="32e11-298">Network</span></span>

* <span data-ttu-id="32e11-299">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="32e11-300">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="32e11-301">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="32e11-302">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="32e11-303">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="32e11-304">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="32e11-305">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="32e11-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="32e11-306">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="32e11-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="32e11-307">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="32e11-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="32e11-308">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="32e11-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="32e11-309">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="32e11-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="32e11-310">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="32e11-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="32e11-311">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="32e11-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="32e11-312">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="32e11-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="32e11-313">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="32e11-314">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="32e11-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="32e11-315">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="32e11-316">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="32e11-317">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="32e11-318">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="32e11-319">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="32e11-320">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="32e11-321">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="32e11-322">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="32e11-323">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="32e11-324">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="32e11-325">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="32e11-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="32e11-326">프로필</span><span class="sxs-lookup"><span data-stu-id="32e11-326">Profile</span></span>

* <span data-ttu-id="32e11-327">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="32e11-328">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="32e11-329">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="32e11-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="32e11-330">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="32e11-331">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="32e11-332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="32e11-332">RDBMS</span></span>

* <span data-ttu-id="32e11-333">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="32e11-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="32e11-334">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="32e11-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="32e11-335">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="32e11-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="32e11-336">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="32e11-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="32e11-337">리소스</span><span class="sxs-lookup"><span data-stu-id="32e11-337">Resource</span></span>

* <span data-ttu-id="32e11-338">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="32e11-339">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="32e11-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="32e11-340">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="32e11-341">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="32e11-342">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="32e11-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="32e11-343">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="32e11-344">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="32e11-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="32e11-345">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="32e11-346">역할</span><span class="sxs-lookup"><span data-stu-id="32e11-346">Role</span></span>

* <span data-ttu-id="32e11-347">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="32e11-348">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="32e11-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="32e11-349">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="32e11-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="32e11-350">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="32e11-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="32e11-351">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="32e11-352">서비스 패브릭</span><span class="sxs-lookup"><span data-stu-id="32e11-352">Service Fabric</span></span>
* <span data-ttu-id="32e11-353">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="32e11-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="32e11-354">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="32e11-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="32e11-355">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="32e11-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="32e11-356">SQL</span><span class="sxs-lookup"><span data-stu-id="32e11-356">SQL</span></span>

* <span data-ttu-id="32e11-357">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="32e11-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="32e11-358">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="32e11-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="32e11-359">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="32e11-360">저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-360">Storage</span></span>

* <span data-ttu-id="32e11-361">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="32e11-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="32e11-362">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="32e11-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="32e11-363">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="32e11-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="32e11-364">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="32e11-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="32e11-365">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="32e11-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="32e11-366">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="32e11-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="32e11-367">VM</span><span class="sxs-lookup"><span data-stu-id="32e11-367">VM</span></span>

* <span data-ttu-id="32e11-368">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-368">Support configuring nsg</span></span>
* <span data-ttu-id="32e11-369">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="32e11-370">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="32e11-370">Support managed service identities</span></span>
* <span data-ttu-id="32e11-371">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="32e11-372">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="32e11-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="32e11-373">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="32e11-373">May 10, 2017</span></span>

<span data-ttu-id="32e11-374">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="32e11-374">Version 2.0.6</span></span>

* <span data-ttu-id="32e11-375">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="32e11-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="32e11-376">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="32e11-377">Data Lake Analytics 및 Data Lake Store 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="32e11-378">Cognitive Services 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="32e11-379">Service Fabric 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="32e11-380">대화형 모듈(az-shell 이름 바꾸기)을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="32e11-381">CDN 명령에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="32e11-382">컨테이너 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-382">Remove Container module.</span></span>
* <span data-ttu-id="32e11-383">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="32e11-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="32e11-384">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="32e11-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="32e11-385">코어</span><span class="sxs-lookup"><span data-stu-id="32e11-385">Core</span></span>

* <span data-ttu-id="32e11-386">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="32e11-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="32e11-387">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="32e11-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="32e11-388">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="32e11-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="32e11-389">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="32e11-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="32e11-390">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="32e11-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="32e11-391">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="32e11-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="32e11-392">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="32e11-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="32e11-393">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="32e11-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="32e11-394">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="32e11-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="32e11-395">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="32e11-395">core: Improved performance</span></span>
* <span data-ttu-id="32e11-396">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="32e11-397">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="32e11-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="32e11-398">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-398">ACS</span></span>

* <span data-ttu-id="32e11-399">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="32e11-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="32e11-400">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="32e11-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="32e11-401">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="32e11-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="32e11-402">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="32e11-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="32e11-403">AppService</span><span class="sxs-lookup"><span data-stu-id="32e11-403">AppService</span></span>

* <span data-ttu-id="32e11-404">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="32e11-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="32e11-405">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="32e11-406">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="32e11-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="32e11-407">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="32e11-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="32e11-408">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="32e11-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="32e11-409">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="32e11-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="32e11-410">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-410">support slot swap with preview</span></span>
* <span data-ttu-id="32e11-411">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="32e11-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="32e11-412">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="32e11-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="32e11-413">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="32e11-413">CosmosDB</span></span>

* <span data-ttu-id="32e11-414">documentdb 모듈 이름을 cosmosdb로 바꿈</span><span class="sxs-lookup"><span data-stu-id="32e11-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="32e11-415">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="32e11-416">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="32e11-417">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="32e11-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="32e11-418">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="32e11-418">Data Lake Analytics</span></span>

* <span data-ttu-id="32e11-419">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="32e11-420">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="32e11-421">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="32e11-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="32e11-422">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="32e11-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="32e11-423">테이블</span><span class="sxs-lookup"><span data-stu-id="32e11-423">Table</span></span>
  * <span data-ttu-id="32e11-424">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="32e11-424">Table valued function</span></span>
  * <span data-ttu-id="32e11-425">보기</span><span class="sxs-lookup"><span data-stu-id="32e11-425">View</span></span>
  * <span data-ttu-id="32e11-426">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="32e11-426">Table Statistics.</span></span> <span data-ttu-id="32e11-427">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="32e11-428">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-428">Data Lake Store</span></span>

* <span data-ttu-id="32e11-429">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 대해 보다 나은 지원을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="32e11-430">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="32e11-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="32e11-431">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="32e11-431">missed help for access show.</span></span> <span data-ttu-id="32e11-432">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-432">adding it.</span></span> <span data-ttu-id="32e11-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="32e11-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="32e11-434">찾기</span><span class="sxs-lookup"><span data-stu-id="32e11-434">Find</span></span>

* <span data-ttu-id="32e11-435">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="32e11-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="32e11-436">KeyVault</span><span class="sxs-lookup"><span data-stu-id="32e11-436">KeyVault</span></span>

* <span data-ttu-id="32e11-437">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="32e11-438">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="32e11-439">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="32e11-440">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="32e11-441">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="32e11-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="32e11-442">랩</span><span class="sxs-lookup"><span data-stu-id="32e11-442">Lab</span></span>

* <span data-ttu-id="32e11-443">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="32e11-444">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="32e11-445">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="32e11-446">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="32e11-447">랩 내에서 비밀을 관리하는 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="32e11-448">모니터</span><span class="sxs-lookup"><span data-stu-id="32e11-448">Monitor</span></span>

* <span data-ttu-id="32e11-449">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="32e11-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="32e11-450">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="32e11-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="32e11-451">네트워크</span><span class="sxs-lookup"><span data-stu-id="32e11-451">Network</span></span>

* <span data-ttu-id="32e11-452">`network watcher test-connectivity` 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="32e11-453">`network watcher packet-capture create`에 대한 `--filters` 매개 변수 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="32e11-454">Application Gateway 연결 드레이닝에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="32e11-455">Application Gateway WAF 규칙 집합 구성에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="32e11-456">ExpressRoute 경로 필터 및 규칙에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="32e11-457">TrafficManager 지리적 라우팅에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="32e11-458">VPN 연결 정책 기반 트래픽 선택기에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="32e11-459">VPN 연결 IPSec 정책에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="32e11-460">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create`를 사용하여 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="32e11-461">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="32e11-462">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="32e11-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="32e11-463">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="32e11-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="32e11-464">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="32e11-465">레코드가 제대로 가져와지지 않는 `dns zone import`의 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="32e11-466">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="32e11-467">'network watcher' 미리 보기 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="32e11-468">프로필</span><span class="sxs-lookup"><span data-stu-id="32e11-468">Profile</span></span>

* <span data-ttu-id="32e11-469">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="32e11-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="32e11-470">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="32e11-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="32e11-471">Redis</span><span class="sxs-lookup"><span data-stu-id="32e11-471">Redis</span></span>

* <span data-ttu-id="32e11-472">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="32e11-473">'update-settings' 명령은 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="32e11-474">리소스</span><span class="sxs-lookup"><span data-stu-id="32e11-474">Resource</span></span>

* <span data-ttu-id="32e11-475">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="32e11-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="32e11-476">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="32e11-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="32e11-477">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="32e11-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="32e11-478">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="32e11-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="32e11-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="32e11-480">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-480">Add docs for az lock update.</span></span> <span data-ttu-id="32e11-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="32e11-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="32e11-482">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="32e11-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="32e11-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="32e11-484">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="32e11-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="32e11-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="32e11-486">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="32e11-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="32e11-487">역할</span><span class="sxs-lookup"><span data-stu-id="32e11-487">Role</span></span>

* <span data-ttu-id="32e11-488">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="32e11-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="32e11-489">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="32e11-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="32e11-490">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="32e11-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="32e11-491">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="32e11-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="32e11-492">SQL</span><span class="sxs-lookup"><span data-stu-id="32e11-492">SQL</span></span>

* <span data-ttu-id="32e11-493">az sql server list-usages 및 az sql db list-usages 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="32e11-494">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="32e11-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="32e11-495">저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-495">Storage</span></span>

* <span data-ttu-id="32e11-496">기본 위치를 `storage account create`에 대한 리소스 그룹 위치로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="32e11-497">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="32e11-498">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="32e11-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="32e11-499">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="32e11-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="32e11-500">VM</span><span class="sxs-lookup"><span data-stu-id="32e11-500">VM</span></span>

* <span data-ttu-id="32e11-501">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="32e11-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="32e11-502">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="32e11-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="32e11-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="32e11-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="32e11-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="32e11-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="32e11-505">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="32e11-506">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="32e11-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="32e11-507">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="32e11-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="32e11-508">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="32e11-508">April 3, 2017</span></span>

<span data-ttu-id="32e11-509">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="32e11-509">Version 2.0.2</span></span>

<span data-ttu-id="32e11-510">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 출시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="32e11-511">코어</span><span class="sxs-lookup"><span data-stu-id="32e11-511">Core</span></span>

* <span data-ttu-id="32e11-512">기본 목록에 acr, 랩, 모니터 및 찾기 모듈을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="32e11-513">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="32e11-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="32e11-514">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="32e11-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="32e11-515">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="32e11-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="32e11-516">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="32e11-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="32e11-517">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="32e11-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="32e11-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="32e11-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="32e11-519">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="32e11-520">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="32e11-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="32e11-521">ACS</span><span class="sxs-lookup"><span data-stu-id="32e11-521">ACS</span></span>

* <span data-ttu-id="32e11-522">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="32e11-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="32e11-523">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="32e11-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="32e11-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="32e11-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="32e11-525">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="32e11-525">Add support for windows clusters.</span></span> <span data-ttu-id="32e11-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="32e11-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="32e11-527">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="32e11-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="32e11-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="32e11-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="32e11-529">AppService</span><span class="sxs-lookup"><span data-stu-id="32e11-529">AppService</span></span>

* <span data-ttu-id="32e11-530">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="32e11-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="32e11-531">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="32e11-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="32e11-532">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="32e11-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="32e11-533">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="32e11-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="32e11-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="32e11-534">DataLake</span></span>

* <span data-ttu-id="32e11-535">Data Lake Analytics 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="32e11-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="32e11-536">Data Lake Store 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="32e11-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="32e11-537">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="32e11-537">DocuemntDB</span></span>

* <span data-ttu-id="32e11-538">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="32e11-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="32e11-539">VM</span><span class="sxs-lookup"><span data-stu-id="32e11-539">VM</span></span>

* <span data-ttu-id="32e11-540">[Compute] 가상 컴퓨터 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="32e11-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="32e11-541">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="32e11-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="32e11-542">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="32e11-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="32e11-543">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="32e11-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="32e11-544">가상 컴퓨터 확장 집합: vm의 인스턴스 보기를 나열하는 * 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="32e11-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="32e11-545">VM 및 가상 컴퓨터 확장 집합에 --secrets 추가([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="32e11-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="32e11-546">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="32e11-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="32e11-547">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="32e11-547">February 27, 2017</span></span>

<span data-ttu-id="32e11-548">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="32e11-548">Version 2.0.0</span></span>

<span data-ttu-id="32e11-549">Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="32e11-550">일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="32e11-551">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="32e11-551">Container Service (acs)</span></span>
- <span data-ttu-id="32e11-552">Compute(Resource Manager, VM, 가상 컴퓨터 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="32e11-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="32e11-553">네트워킹</span><span class="sxs-lookup"><span data-stu-id="32e11-553">Networking</span></span>
- <span data-ttu-id="32e11-554">저장소</span><span class="sxs-lookup"><span data-stu-id="32e11-554">Storage</span></span>

<span data-ttu-id="32e11-555">이러한 명령은 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="32e11-556">Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 개설할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="32e11-557">[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="32e11-558">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="32e11-559">CLI 버전을 확인하려면 `az --version`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="32e11-560">출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="32e11-561">일부 명령 모듈에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="32e11-562">이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="32e11-563">CLI 야간 미리 보기 빌드도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="32e11-564">자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="32e11-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="32e11-565">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32e11-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="32e11-566">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="32e11-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="32e11-567">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.</span><span class="sxs-lookup"><span data-stu-id="32e11-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="32e11-568">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공.</span><span class="sxs-lookup"><span data-stu-id="32e11-568">Provide feedback from the command line with the `az feedback` command.</span></span>

